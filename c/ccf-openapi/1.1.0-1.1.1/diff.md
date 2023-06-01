# Comparing `tmp/ccf-openapi-1.1.0.tar.gz` & `tmp/ccf-openapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccf-openapi-1.1.0.tar", last modified: Fri Jun 17 17:52:31 2022, max compression
+gzip compressed data, was "ccf-openapi-1.1.1.tar", last modified: Wed May 31 11:04:13 2023, max compression
```

## Comparing `ccf-openapi-1.1.0.tar` & `ccf-openapi-1.1.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      461 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/PKG-INFO
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     9267 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/README.md
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.733011 ccf-openapi-1.1.0/ccf_openapi.egg-info/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      461 2022-06-17 17:52:31.000000 ccf-openapi-1.1.0/ccf_openapi.egg-info/PKG-INFO
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     2880 2022-06-17 17:52:31.000000 ccf-openapi-1.1.0/ccf_openapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bherr     (1000) bherr     (1000)        1 2022-06-17 17:52:31.000000 ccf-openapi-1.1.0/ccf_openapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bherr     (1000) bherr     (1000)       32 2022-06-17 17:52:31.000000 ccf-openapi-1.1.0/ccf_openapi.egg-info/requires.txt
--rw-rw-r--   0 bherr     (1000) bherr     (1000)       19 2022-06-17 17:52:31.000000 ccf-openapi-1.1.0/ccf_openapi.egg-info/top_level.txt
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.733011 ccf-openapi-1.1.0/ccf_openapi_client/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      843 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/__init__.py
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.733011 ccf-openapi-1.1.0/ccf_openapi_client/api/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      222 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/api/__init__.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)   104797 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/api/default_api.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    37730 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/api_client.py
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.733011 ccf-openapi-1.1.0/ccf_openapi_client/apis/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      471 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/apis/__init__.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    16538 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/configuration.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     5133 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/exceptions.py
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/ccf_openapi_client/model/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      348 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/__init__.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11517 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/aggregate_count.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12071 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/database_status.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11101 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/error_message.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    16423 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/flat_spatial_placement.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11725 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/get_spatial_placement_request.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    10908 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/json_ld_object.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11248 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/min_max.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11740 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/ontology_tree.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    14135 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/ontology_tree_node.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11436 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/rgba.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11157 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/sparql_query_request.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    19750 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12260 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12065 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_creator.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12363 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_dimensions.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    13614 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_object_reference.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    16729 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    16850 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12280 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_rotation.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12183 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_scaling.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    12467 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_translation.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    18057 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_scene_node.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11800 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_search.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    16360 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_block.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11596 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    13954 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_dataset.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    13809 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_donor.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    11673 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_sample_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    14617 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_section.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    82151 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/model_utils.py
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/ccf_openapi_client/models/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     2495 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/models/__init__.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)    14261 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/ccf_openapi_client/rest.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)       69 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/setup.cfg
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1167 2022-06-17 17:51:48.000000 ccf-openapi-1.1.0/setup.py
-drwxrwxr-x   0 bherr     (1000) bherr     (1000)        0 2022-06-17 17:52:31.737011 ccf-openapi-1.1.0/test/
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      833 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_aggregate_count.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      833 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_database_status.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     3573 2022-06-17 17:42:15.000000 ccf-openapi-1.1.0/test/test_default_api.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      819 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_error_message.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1022 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_flat_spatial_placement.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1028 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_get_spatial_placement_request.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      820 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_json_ld_object.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      777 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_min_max.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      941 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_ontology_tree.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      954 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_ontology_tree_node.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      762 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_rgba.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      862 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_sparql_query_request.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1572 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_entity.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      869 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_entity_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      876 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_entity_creator.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      897 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_entity_dimensions.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      996 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_object_reference.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1102 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_placement.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1466 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_placement_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      904 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_placement_rotation.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      897 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_placement_scaling.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      925 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_placement_translation.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1160 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_scene_node.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      826 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_spatial_search.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1472 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_block.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      819 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1037 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_dataset.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1023 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_donor.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)      971 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_sample_common.py
--rw-rw-r--   0 bherr     (1000) bherr     (1000)     1276 2022-06-17 17:42:14.000000 ccf-openapi-1.1.0/test/test_tissue_section.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     9274 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/README.md
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi.egg-info/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      449 2023-05-31 11:04:13.000000 ccf-openapi-1.1.1/ccf_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2880 2023-05-31 11:04:13.000000 ccf-openapi-1.1.1/ccf_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)        1 2023-05-31 11:04:13.000000 ccf-openapi-1.1.1/ccf_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       32 2023-05-31 11:04:13.000000 ccf-openapi-1.1.1/ccf_openapi.egg-info/requires.txt
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       19 2023-05-31 11:04:13.000000 ccf-openapi-1.1.1/ccf_openapi.egg-info/top_level.txt
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi_client/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      850 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/__init__.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi_client/api/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      222 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/api/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)   104876 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/api/default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    37737 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/api_client.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi_client/apis/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      471 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/apis/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16559 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/configuration.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     5140 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/exceptions.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi_client/model/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      348 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11524 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12078 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11108 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16430 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11732 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    10915 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11255 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11747 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14142 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11443 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11164 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    19757 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12267 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12072 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12370 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13621 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16736 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16857 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12287 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12190 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    12474 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    18061 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11807 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    16417 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11549 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14011 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    13866 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    11680 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14674 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_section.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    82158 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/model_utils.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/ccf_openapi_client/models/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     2495 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/models/__init__.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)    14268 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/ccf_openapi_client/rest.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)       69 2023-05-31 11:04:13.791277 ccf-openapi-1.1.1/setup.cfg
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1181 2023-05-31 11:02:59.000000 ccf-openapi-1.1.1/setup.py
+drwxr-xr-x   0 bherr     (1000) bherr     (1000)        0 2023-05-31 11:04:13.780443 ccf-openapi-1.1.1/test/
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_aggregate_count.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      840 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_database_status.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     3580 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_default_api.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_error_message.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1029 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_flat_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1035 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_get_spatial_placement_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      827 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_json_ld_object.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      784 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_min_max.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      948 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_ontology_tree.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      961 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_ontology_tree_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      769 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_rgba.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      869 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_sparql_query_request.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1579 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_spatial_entity.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      876 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_spatial_entity_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      883 2023-05-31 11:00:01.000000 ccf-openapi-1.1.1/test/test_spatial_entity_creator.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_entity_dimensions.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1003 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_object_reference.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1109 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_placement.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1473 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_placement_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      911 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_placement_rotation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      904 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_placement_scaling.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      932 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_placement_translation.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1167 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_scene_node.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      833 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_spatial_search.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1479 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_block.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      826 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1044 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_dataset.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1030 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_donor.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)      978 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_sample_common.py
+-rw-r--r--   0 bherr     (1000) bherr     (1000)     1283 2023-05-31 11:00:02.000000 ccf-openapi-1.1.1/test/test_tissue_section.py
```

### Comparing `ccf-openapi-1.1.0/README.md` & `ccf-openapi-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ccf-openapi
-This API provides programmatic access to data registered to the CCF.
-See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.
+This API provides programmatic access to data registered to the Human Reference Atlas (HRA).
+See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
 - Package version: 1.0.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi.egg-info/SOURCES.txt` & `ccf-openapi-1.1.1/ccf_openapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/__init__.py` & `ccf-openapi-1.1.1/ccf_openapi_client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/api/default_api.py` & `ccf-openapi-1.1.1/ccf_openapi_client/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -1025,15 +1025,15 @@
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.sparql_endpoint = _Endpoint(
             settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'response_type': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
                 'auth': [],
                 'endpoint_path': '/sparql',
                 'operation_id': 'sparql',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
@@ -1095,23 +1095,24 @@
                     'format': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/json',
+                    'text/csv'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
         self.sparql_post_endpoint = _Endpoint(
             settings={
-                'response_type': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},),
+                'response_type': ([{str: (bool, date, datetime, dict, float, int, list, str, none_type)}],),
                 'auth': [],
                 'endpoint_path': '/sparql',
                 'operation_id': 'sparql_post',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
@@ -1172,15 +1173,16 @@
                     'format': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
-                    'application/json'
+                    'application/json',
+                    'text/csv'
                 ],
                 'content_type': [
                     'application/json',
                     'application/x-www-form-urlencoded'
                 ]
             },
             api_client=api_client
@@ -2415,15 +2417,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+            [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
@@ -2494,15 +2496,15 @@
                 content-types and body.
             _host_index (int/None): specifies the index of the server
                 that we want to use.
                 Default is read from the configuration.
             async_req (bool): execute request asynchronously
 
         Returns:
-            {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+            [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
                 If the method is called asynchronously, returns the request
                 thread.
         """
         kwargs['async_req'] = kwargs.get(
             'async_req', False
         )
         kwargs['_return_http_data_only'] = kwargs.get(
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/api_client.py` & `ccf-openapi-1.1.1/ccf_openapi_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/configuration.py` & `ccf-openapi-1.1.1/ccf_openapi_client/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
@@ -390,19 +390,19 @@
         """
         return [
             {
                 'url': "/v1",
                 'description': "CCF-API",
             },
             {
-                'url': "https://ccf-api.herokuapp.com/v1",
+                'url': "https://ccf-api.hubmapconsortium.org/v1",
                 'description': "Production Server (backup)",
             },
             {
-                'url': "https://ccf-api--staging.herokuapp.com/v1",
+                'url': "https://r5i95k35v5.us-east-2.awsapprunner.com/v1",
                 'description': "Staging Server",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/exceptions.py` & `ccf-openapi-1.1.1/ccf_openapi_client/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/aggregate_count.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/aggregate_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/database_status.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/database_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/error_message.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/error_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/flat_spatial_placement.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/flat_spatial_placement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/get_spatial_placement_request.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/get_spatial_placement_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/json_ld_object.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/json_ld_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/min_max.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/min_max.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/ontology_tree.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/ontology_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/ontology_tree_node.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/ontology_tree_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/rgba.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/rgba.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/sparql_query_request.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/sparql_query_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_common.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_creator.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_entity_dimensions.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_entity_dimensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_object_reference.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_object_reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_common.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_rotation.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_scaling.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_placement_translation.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_placement_translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_scene_node.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_scene_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -95,15 +95,15 @@
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'tooltip': (str,),  # noqa: E501
             'unpickable': (bool,),  # noqa: E501
             'geometry': (str,),  # noqa: E501
-            'lighting': (bool,),  # noqa: E501
+            'lighting': (str,),  # noqa: E501
             'zoom_based_opacity': (bool,),  # noqa: E501
             'zoom_to_on_load': (bool,),  # noqa: E501
             'scenegraph': (str,),  # noqa: E501
             'scenegraph_node': (str,),  # noqa: E501
             'color': (Rgba,),  # noqa: E501
             'opacity': (float,),  # noqa: E501
             'transform_matrix': ([float],),  # noqa: E501
@@ -178,15 +178,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): [optional]  # noqa: E501
             tooltip (str): [optional]  # noqa: E501
             unpickable (bool): Whether the node should selectable by the user in interfaces.. [optional]  # noqa: E501
             geometry (str): Geometry to draw, if it is not using a GLTF file.. [optional]  # noqa: E501
-            lighting (bool): [optional]  # noqa: E501
+            lighting (str): [optional]  # noqa: E501
             zoom_based_opacity (bool): Whether the opacity of the node changes based on the zoom level.. [optional]  # noqa: E501
             zoom_to_on_load (bool): Focus this node when loaded in an interface.. [optional]  # noqa: E501
             scenegraph (str): [optional]  # noqa: E501
             scenegraph_node (str): [optional]  # noqa: E501
             color (Rgba): [optional]  # noqa: E501
             opacity (float): [optional]  # noqa: E501
             transform_matrix ([float]): Additional transformations to be applied.. [optional]  # noqa: E501
@@ -294,15 +294,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): [optional]  # noqa: E501
             tooltip (str): [optional]  # noqa: E501
             unpickable (bool): Whether the node should selectable by the user in interfaces.. [optional]  # noqa: E501
             geometry (str): Geometry to draw, if it is not using a GLTF file.. [optional]  # noqa: E501
-            lighting (bool): [optional]  # noqa: E501
+            lighting (str): [optional]  # noqa: E501
             zoom_based_opacity (bool): Whether the opacity of the node changes based on the zoom level.. [optional]  # noqa: E501
             zoom_to_on_load (bool): Focus this node when loaded in an interface.. [optional]  # noqa: E501
             scenegraph (str): [optional]  # noqa: E501
             scenegraph_node (str): [optional]  # noqa: E501
             color (Rgba): [optional]  # noqa: E501
             opacity (float): [optional]  # noqa: E501
             transform_matrix ([float]): Additional transformations to be applied.. [optional]  # noqa: E501
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/spatial_search.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/spatial_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_block.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -107,17 +107,17 @@
             'spatial_entity_id': (str,),  # noqa: E501
             'donor': (TissueDonor,),  # noqa: E501
             'section_count': (int,),  # noqa: E501
             'section_size': (float,),  # noqa: E501
             'section_units': (str,),  # noqa: E501
             'sections': ([TissueSection],),  # noqa: E501
             'label': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
             'datasets': ([TissueDataset],),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -126,17 +126,17 @@
         'spatial_entity_id': 'spatialEntityId',  # noqa: E501
         'donor': 'donor',  # noqa: E501
         'section_count': 'sectionCount',  # noqa: E501
         'section_size': 'sectionSize',  # noqa: E501
         'section_units': 'sectionUnits',  # noqa: E501
         'sections': 'sections',  # noqa: E501
         'label': 'label',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'link': 'link',  # noqa: E501
         'datasets': 'datasets',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
@@ -148,15 +148,14 @@
             spatial_entity_id (str): The associated spatial entity (rui_location) for the block.
             donor (TissueDonor):
             section_count (int): Number of sections contained in the block.
             section_size (float): Size of each section in the block.
             section_units (str): Length unit `sectionSize` is in (generally, millimeters). defaults to "millimeters"  # noqa: E501
             sections ([TissueSection]): All sections in the block.
             label (str):
-            description (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -181,14 +180,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         section_units = kwargs.get('section_units', "millimeters")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -259,15 +259,14 @@
             spatial_entity_id (str): The associated spatial entity (rui_location) for the block.
             donor (TissueDonor):
             section_count (int): Number of sections contained in the block.
             section_size (float): Size of each section in the block.
             section_units (str): Length unit `sectionSize` is in (generally, millimeters). defaults to "millimeters"  # noqa: E501
             sections ([TissueSection]): All sections in the block.
             label (str):
-            description (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -292,14 +291,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         section_units = kwargs.get('section_units', "millimeters")
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_common.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -78,42 +78,41 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'label': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'label': 'label',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'link': 'link',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, label, description, link, *args, **kwargs):  # noqa: E501
+    def _from_openapi_data(cls, label, link, *args, **kwargs):  # noqa: E501
         """TissueCommon - a model defined in OpenAPI
 
         Args:
             label (str):
-            description (str):
             link (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -139,14 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -167,15 +167,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.label = label
-        self.description = description
         self.link = link
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
@@ -189,20 +188,19 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, label, description, link, *args, **kwargs):  # noqa: E501
+    def __init__(self, label, link, *args, **kwargs):  # noqa: E501
         """TissueCommon - a model defined in OpenAPI
 
         Args:
             label (str):
-            description (str):
             link (str):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -228,14 +226,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -254,15 +253,14 @@
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.label = label
-        self.description = description
         self.link = link
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_dataset.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -88,44 +88,43 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'technology': (str,),  # noqa: E501
             'thumbnail': (str,),  # noqa: E501
             'label': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'technology': 'technology',  # noqa: E501
         'thumbnail': 'thumbnail',  # noqa: E501
         'label': 'label',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'link': 'link',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TissueDataset - a model defined in OpenAPI
 
         Keyword Args:
             technology (str):
             thumbnail (str):
             label (str):
-            description (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -149,14 +148,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -221,15 +221,14 @@
     def __init__(self, *args, **kwargs):  # noqa: E501
         """TissueDataset - a model defined in OpenAPI
 
         Keyword Args:
             technology (str):
             thumbnail (str):
             label (str):
-            description (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -253,14 +252,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_donor.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_donor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -87,42 +87,41 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'provider_name': (str,),  # noqa: E501
             'label': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'provider_name': 'providerName',  # noqa: E501
         'label': 'label',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'link': 'link',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TissueDonor - a model defined in OpenAPI
 
         Keyword Args:
             provider_name (str):
             label (str):
-            description (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -146,14 +145,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -217,15 +217,14 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
         """TissueDonor - a model defined in OpenAPI
 
         Keyword Args:
             provider_name (str):
             label (str):
-            description (str):
             link (str):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
@@ -249,14 +248,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_sample_common.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_sample_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model/tissue_section.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model/tissue_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
@@ -95,46 +95,45 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'sample_type': (str,),  # noqa: E501
             'section_number': (int,),  # noqa: E501
             'label': (str,),  # noqa: E501
-            'description': (str,),  # noqa: E501
             'link': (str,),  # noqa: E501
             'datasets': ([TissueDataset],),  # noqa: E501
+            'description': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'sample_type': 'sampleType',  # noqa: E501
         'section_number': 'sectionNumber',  # noqa: E501
         'label': 'label',  # noqa: E501
-        'description': 'description',  # noqa: E501
         'link': 'link',  # noqa: E501
         'datasets': 'datasets',  # noqa: E501
+        'description': 'description',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
         """TissueSection - a model defined in OpenAPI
 
         Keyword Args:
             sample_type (str):
             section_number (int): Index of the section in the parent block.
             label (str):
-            description (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -159,14 +158,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -231,15 +231,14 @@
     def __init__(self, *args, **kwargs):  # noqa: E501
         """TissueSection - a model defined in OpenAPI
 
         Keyword Args:
             sample_type (str):
             section_number (int): Index of the section in the parent block.
             label (str):
-            description (str):
             link (str):
             datasets ([TissueDataset]):
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -264,14 +263,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            description (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/model_utils.py` & `ccf-openapi-1.1.1/ccf_openapi_client/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
```

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/models/__init__.py` & `ccf-openapi-1.1.1/ccf_openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ccf-openapi-1.1.0/ccf_openapi_client/rest.py` & `ccf-openapi-1.1.1/ccf_openapi_client/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
```

### Comparing `ccf-openapi-1.1.0/setup.py` & `ccf-openapi-1.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "ccf-openapi"
-VERSION = "1.1.0"
+VERSION = "1.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -33,10 +33,10 @@
     url="",
     keywords=["OpenAPI", "OpenAPI-Generator", "CCF-API"],
     python_requires=">=3.6",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description="""\
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
     """
 )
```

### Comparing `ccf-openapi-1.1.0/test/test_aggregate_count.py` & `ccf-openapi-1.1.1/test/test_aggregate_count.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_database_status.py` & `ccf-openapi-1.1.1/test/test_database_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_default_api.py` & `ccf-openapi-1.1.1/test/test_default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import unittest
```

### Comparing `ccf-openapi-1.1.0/test/test_error_message.py` & `ccf-openapi-1.1.1/test/test_error_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_flat_spatial_placement.py` & `ccf-openapi-1.1.1/test/test_flat_spatial_placement.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_get_spatial_placement_request.py` & `ccf-openapi-1.1.1/test/test_get_spatial_placement_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_json_ld_object.py` & `ccf-openapi-1.1.1/test/test_json_ld_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_min_max.py` & `ccf-openapi-1.1.1/test/test_min_max.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_ontology_tree.py` & `ccf-openapi-1.1.1/test/test_ontology_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_ontology_tree_node.py` & `ccf-openapi-1.1.1/test/test_ontology_tree_node.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_rgba.py` & `ccf-openapi-1.1.1/test/test_sparql_query_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ccf_openapi_client
-from ccf_openapi_client.model.rgba import Rgba
+from ccf_openapi_client.model.sparql_query_request import SparqlQueryRequest
 
 
-class TestRgba(unittest.TestCase):
-    """Rgba unit test stubs"""
+class TestSparqlQueryRequest(unittest.TestCase):
+    """SparqlQueryRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRgba(self):
-        """Test Rgba"""
+    def testSparqlQueryRequest(self):
+        """Test SparqlQueryRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = Rgba()  # noqa: E501
+        # model = SparqlQueryRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_entity.py` & `ccf-openapi-1.1.1/test/test_spatial_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_entity_common.py` & `ccf-openapi-1.1.1/test/test_spatial_entity_common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_entity_creator.py` & `ccf-openapi-1.1.1/test/test_spatial_entity_creator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_entity_dimensions.py` & `ccf-openapi-1.1.1/test/test_spatial_entity_dimensions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_object_reference.py` & `ccf-openapi-1.1.1/test/test_spatial_object_reference.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_placement.py` & `ccf-openapi-1.1.1/test/test_spatial_placement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_placement_common.py` & `ccf-openapi-1.1.1/test/test_spatial_placement_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_placement_rotation.py` & `ccf-openapi-1.1.1/test/test_spatial_placement_rotation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_placement_scaling.py` & `ccf-openapi-1.1.1/test/test_spatial_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ccf_openapi_client
-from ccf_openapi_client.model.spatial_placement_scaling import SpatialPlacementScaling
+from ccf_openapi_client.model.spatial_search import SpatialSearch
 
 
-class TestSpatialPlacementScaling(unittest.TestCase):
-    """SpatialPlacementScaling unit test stubs"""
+class TestSpatialSearch(unittest.TestCase):
+    """SpatialSearch unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSpatialPlacementScaling(self):
-        """Test SpatialPlacementScaling"""
+    def testSpatialSearch(self):
+        """Test SpatialSearch"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SpatialPlacementScaling()  # noqa: E501
+        # model = SpatialSearch()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_placement_translation.py` & `ccf-openapi-1.1.1/test/test_spatial_placement_translation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_scene_node.py` & `ccf-openapi-1.1.1/test/test_spatial_scene_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_spatial_search.py` & `ccf-openapi-1.1.1/test/test_spatial_placement_scaling.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
 import unittest
 
 import ccf_openapi_client
-from ccf_openapi_client.model.spatial_search import SpatialSearch
+from ccf_openapi_client.model.spatial_placement_scaling import SpatialPlacementScaling
 
 
-class TestSpatialSearch(unittest.TestCase):
-    """SpatialSearch unit test stubs"""
+class TestSpatialPlacementScaling(unittest.TestCase):
+    """SpatialPlacementScaling unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSpatialSearch(self):
-        """Test SpatialSearch"""
+    def testSpatialPlacementScaling(self):
+        """Test SpatialPlacementScaling"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = SpatialSearch()  # noqa: E501
+        # model = SpatialPlacementScaling()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_block.py` & `ccf-openapi-1.1.1/test/test_tissue_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_common.py` & `ccf-openapi-1.1.1/test/test_tissue_common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_dataset.py` & `ccf-openapi-1.1.1/test/test_tissue_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_donor.py` & `ccf-openapi-1.1.1/test/test_tissue_donor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_sample_common.py` & `ccf-openapi-1.1.1/test/test_tissue_sample_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

### Comparing `ccf-openapi-1.1.0/test/test_tissue_section.py` & `ccf-openapi-1.1.1/test/test_tissue_section.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
     CCF-API
 
-    This API provides programmatic access to data registered to the CCF. See the [HuBMAP CCF Portal](https://hubmapconsortium.github.io/ccf/) for details.   # noqa: E501
+    This API provides programmatic access to data registered to the Human Reference Atlas (HRA). See the [HuBMAP HRA Portal](https://humanatlas.io/) for details.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import sys
```

