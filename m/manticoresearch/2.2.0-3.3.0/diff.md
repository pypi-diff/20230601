# Comparing `tmp/manticoresearch-2.2.0.tar.gz` & `tmp/manticoresearch-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manticoresearch-2.2.0.tar", last modified: Thu Jun  2 13:06:27 2022, max compression
+gzip compressed data, was "manticoresearch-3.3.0.tar", last modified: Thu Jun  1 06:08:43 2023, max compression
```

## Comparing `manticoresearch-2.2.0.tar` & `manticoresearch-3.3.0.tar`

### file list

```diff
@@ -1,49 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.048822 manticoresearch-2.2.0/
--rwxrwxrwx   0 root         (0) root         (0)     1095 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3881 2022-06-02 13:06:27.048822 manticoresearch-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4394 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.039656 manticoresearch-2.2.0/manticoresearch/
--rw-rw-rw-   0 root         (0) root         (0)     1965 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.042405 manticoresearch-2.2.0/manticoresearch/api/
--rw-rw-rw-   0 root         (0) root         (0)      242 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37191 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/api/index_api.py
--rw-rw-rw-   0 root         (0) root         (0)    16491 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/api/search_api.py
--rw-rw-rw-   0 root         (0) root         (0)     8401 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/api/utils_api.py
--rw-rw-rw-   0 root         (0) root         (0)    27322 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.042405 manticoresearch-2.2.0/manticoresearch/apis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15804 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4282 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.046072 manticoresearch-2.2.0/manticoresearch/model/
--rw-rw-rw-   0 root         (0) root         (0)     1310 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3977 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/bulk_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5778 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/delete_document_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5024 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/delete_response.py
--rw-rw-rw-   0 root         (0) root         (0)     4318 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/error_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5925 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/insert_document_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3414 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/percolate_request.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/percolate_request_query.py
--rw-rw-rw-   0 root         (0) root         (0)    11792 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/search_request.py
--rw-rw-rw-   0 root         (0) root         (0)     7159 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/search_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5558 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/search_response_hits.py
--rw-rw-rw-   0 root         (0) root         (0)     2566 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/sql_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5665 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/success_response.py
--rw-rw-rw-   0 root         (0) root         (0)     5975 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/update_document_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5024 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model/update_response.py
--rw-rw-rw-   0 root         (0) root         (0)    82504 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.046989 manticoresearch-2.2.0/manticoresearch/models/
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12196 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/manticoresearch/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.040572 manticoresearch-2.2.0/manticoresearch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3881 2022-06-02 13:06:26.000000 manticoresearch-2.2.0/manticoresearch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1331 2022-06-02 13:06:27.000000 manticoresearch-2.2.0/manticoresearch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-02 13:06:26.000000 manticoresearch-2.2.0/manticoresearch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2022-06-02 13:06:26.000000 manticoresearch-2.2.0/manticoresearch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2022-06-02 13:06:26.000000 manticoresearch-2.2.0/manticoresearch.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-06-02 13:06:27.049739 manticoresearch-2.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2212 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 13:06:27.048822 manticoresearch-2.2.0/test/
--rwxrwxrwx   0 root         (0) root         (0)      933 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/test/test.py
--rwxrwxrwx   0 root         (0) root         (0)     6204 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/test/test_index_api.py
--rwxrwxrwx   0 root         (0) root         (0)     9848 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/test/test_manual.py
--rwxrwxrwx   0 root         (0) root         (0)     3485 2022-06-02 13:06:17.000000 manticoresearch-2.2.0/test/test_search_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.529648 manticoresearch-3.3.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1095 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-06-01 06:08:43.529648 manticoresearch-3.3.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6004 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.519648 manticoresearch-3.3.0/manticoresearch/
+-rwxrwxrwx   0 root         (0) root         (0)     3745 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.521648 manticoresearch-3.3.0/manticoresearch/api/
+-rwxrwxrwx   0 root         (0) root         (0)      242 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37996 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/api/index_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    18561 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/api/search_api.py
+-rwxrwxrwx   0 root         (0) root         (0)     8401 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/api/utils_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    27322 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.521648 manticoresearch-3.3.0/manticoresearch/apis/
+-rwxrwxrwx   0 root         (0) root         (0)      579 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/apis/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    15804 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/configuration.py
+-rwxrwxrwx   0 root         (0) root         (0)     4282 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.528648 manticoresearch-3.3.0/manticoresearch/model/
+-rwxrwxrwx   0 root         (0) root         (0)     3090 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4656 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/aggregation.py
+-rwxrwxrwx   0 root         (0) root         (0)     2566 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/attr_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5129 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/bool_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     3997 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/bulk_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     5814 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/delete_document_request.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/delete_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     3636 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/equals_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     4338 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/error_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     4726 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/facet.py
+-rwxrwxrwx   0 root         (0) root         (0)     5287 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/filter_boolean.py
+-rwxrwxrwx   0 root         (0) root         (0)     5274 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/filter_number.py
+-rwxrwxrwx   0 root         (0) root         (0)     5268 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/filter_string.py
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/fulltext_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     6414 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/geo_distance_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     4190 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/geo_distance_filter_location_anchor.py
+-rwxrwxrwx   0 root         (0) root         (0)    20838 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/highlight.py
+-rwxrwxrwx   0 root         (0) root         (0)     5601 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/highlight_field.py
+-rwxrwxrwx   0 root         (0) root         (0)     3613 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/in_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5961 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/insert_document_request.py
+-rwxrwxrwx   0 root         (0) root         (0)     3743 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/match_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     3608 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/match_op.py
+-rwxrwxrwx   0 root         (0) root         (0)     4995 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/match_op_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     3825 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/match_phrase_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5335 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/not_filter_boolean.py
+-rwxrwxrwx   0 root         (0) root         (0)     5322 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/not_filter_number.py
+-rwxrwxrwx   0 root         (0) root         (0)     5316 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/not_filter_string.py
+-rwxrwxrwx   0 root         (0) root         (0)     2550 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/option.py
+-rwxrwxrwx   0 root         (0) root         (0)     3426 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/percolate_request.py
+-rwxrwxrwx   0 root         (0) root         (0)     3698 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/percolate_request_query.py
+-rwxrwxrwx   0 root         (0) root         (0)     3486 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/query_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)     5080 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/range_filter.py
+-rwxrwxrwx   0 root         (0) root         (0)    15677 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/search_request.py
+-rwxrwxrwx   0 root         (0) root         (0)     7211 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/search_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     5594 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/search_response_hits.py
+-rwxrwxrwx   0 root         (0) root         (0)     4351 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/sort_multiple.py
+-rwxrwxrwx   0 root         (0) root         (0)     4775 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/sort_mva.py
+-rwxrwxrwx   0 root         (0) root         (0)     3718 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/sort_order.py
+-rwxrwxrwx   0 root         (0) root         (0)     4260 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/source_by_rules.py
+-rwxrwxrwx   0 root         (0) root         (0)     2582 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/source_multiple.py
+-rwxrwxrwx   0 root         (0) root         (0)     2570 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/sql_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     5709 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/success_response.py
+-rwxrwxrwx   0 root         (0) root         (0)     6010 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/update_document_request.py
+-rwxrwxrwx   0 root         (0) root         (0)     5060 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model/update_response.py
+-rwxrwxrwx   0 root         (0) root         (0)    82604 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.528648 manticoresearch-3.3.0/manticoresearch/models/
+-rwxrwxrwx   0 root         (0) root         (0)     3137 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/models/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12196 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/manticoresearch/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.520648 manticoresearch-3.3.0/manticoresearch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4313 2023-06-01 06:08:43.000000 manticoresearch-3.3.0/manticoresearch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-06-01 06:08:43.000000 manticoresearch-3.3.0/manticoresearch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:08:43.000000 manticoresearch-3.3.0/manticoresearch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-01 06:08:43.000000 manticoresearch-3.3.0/manticoresearch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 06:08:43.000000 manticoresearch-3.3.0/manticoresearch.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       69 2023-06-01 06:08:43.530648 manticoresearch-3.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2212 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:08:43.529648 manticoresearch-3.3.0/test/
+-rwxrwxrwx   0 root         (0) root         (0)      933 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/test/test.py
+-rwxrwxrwx   0 root         (0) root         (0)     6204 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/test/test_index_api.py
+-rwxrwxrwx   0 root         (0) root         (0)    16378 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/test/test_manual.py
+-rwxrwxrwx   0 root         (0) root         (0)     3485 2023-06-01 06:08:35.000000 manticoresearch-3.3.0/test/test_search_api.py
```

### Comparing `manticoresearch-2.2.0/LICENSE.txt` & `manticoresearch-3.3.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020-2022, Manticore Software LTD 
+Copyright (c) 2020-2023, Manticore Software LTD 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `manticoresearch-2.2.0/PKG-INFO` & `manticoresearch-3.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: manticoresearch
-Version: 2.2.0
+Version: 3.3.0
 Summary: Python client for Manticore Search
-Home-page: UNKNOWN
+Home-page: 
 Author: Manticore Software Ltd.
 Author-email: info@manticoresearch.com
 License: MIT
 Project-URL: Documentation, https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs
 Project-URL: Source Code, https://github.com/manticoresoftware/manticoresearch-python
 Project-URL: Issue Tracker, https://github.com/manticoresoftware/manticoresearch-python/issues
 Keywords: full-text search,manticoresearch,search
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -26,30 +25,27 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # manticoresearch
-Low-level client for Manticore Search.
+Сlient for Manticore Search.
 
 
-❗ WARNING: this is a development version of the client. The latest release's readme is https://github.com/manticoresoftware/manticoresearch-python/tree/2.2.0
 
 ## Requirements.
 
-Python 2.7 and 3.4+.
-
-Minimum Manticore Search version is > 2.5.1 with HTTP protocol enabled.
+Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
 | >= 4.2.1          | 2.0.x                    | >= 3.4        |
-| >= 4.0.2          | 1.0.6                    | >= 3.4        |
-| >= 2.5.1          | 1.0.5                    | >= 2.7        |
+| >= 4.0.2  < 4.2.1 | 1.0.6                    | >= 3.4        |
+| >= 2.5.1  < 4.0.2 | 1.0.5                    | >= 2.7        |
 
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
@@ -94,29 +90,43 @@
     host = "http://127.0.0.1:9308"
 )
 
 
 
 # Enter a context with an instance of the API client
 with manticoresearch.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
+    # Create an instance of the IndexApi API class
     api_instance = manticoresearch.IndexApi(api_client)
     body = "["'{\"insert\": {\"index\": \"test\", \"id\": 1, \"doc\": {\"title\": \"Title 1\"}}},\\n{\"insert\": {\"index\": \"test\", \"id\": 2, \"doc\": {\"title\": \"Title 2\"}}}'"]" # str | 
 
     try:
         # Bulk index operations
         api_response = api_instance.bulk(body)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling IndexApi->bulk: %s\n" % e)
     
+    
+    # Create an instance of the Search API class
+    api_instance = manticoresearch.SearchApi(api_client)
+
+    # Create SearchRequest
+    search_request = SearchRequest()
+    search_request.index='test'
+    search_request.fullltext_filter=QueryFilter('Title 1') 
+    
+    # The example passes only required values which don't have defaults set
+    try:
+        # Perform a search
+        api_response = api_instance.search(search_request)
+        pprint(api_response)
+    except manticoresearch.ApiException as e:
+        print("Exception when calling SearchApi->search: %s\n" % e)
 ```
 
 # Documentation
 
 
-Full documentation is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder.
+Full documentation on the API Endpoints and Models used is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder as listed below.
 
 Manticore Search server documentation: https://manual.manticoresearch.com.
 
-
-
```

### Comparing `manticoresearch-2.2.0/README.md` & `manticoresearch-3.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # manticoresearch
-Low-level client for Manticore Search.
+Сlient for Manticore Search.
 
 
-❗ WARNING: this is a development version of the client. The latest release's readme is https://github.com/manticoresoftware/manticoresearch-python/tree/2.2.0
 
 ## Requirements.
 
-Python 2.7 and 3.4+.
-
-Minimum Manticore Search version is > 2.5.1 with HTTP protocol enabled.
+Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
 | >= 4.2.1          | 2.0.x                    | >= 3.4        |
-| >= 4.0.2          | 1.0.6                    | >= 3.4        |
-| >= 2.5.1          | 1.0.5                    | >= 2.7        |
+| >= 4.0.2  < 4.2.1 | 1.0.6                    | >= 3.4        |
+| >= 2.5.1  < 4.0.2 | 1.0.5                    | >= 2.7        |
 
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
@@ -63,62 +60,107 @@
     host = "http://127.0.0.1:9308"
 )
 
 
 
 # Enter a context with an instance of the API client
 with manticoresearch.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
+    # Create an instance of the IndexApi API class
     api_instance = manticoresearch.IndexApi(api_client)
     body = "["'{\"insert\": {\"index\": \"test\", \"id\": 1, \"doc\": {\"title\": \"Title 1\"}}},\\n{\"insert\": {\"index\": \"test\", \"id\": 2, \"doc\": {\"title\": \"Title 2\"}}}'"]" # str | 
 
     try:
         # Bulk index operations
         api_response = api_instance.bulk(body)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling IndexApi->bulk: %s\n" % e)
     
+    
+    # Create an instance of the Search API class
+    api_instance = manticoresearch.SearchApi(api_client)
+
+    # Create SearchRequest
+    search_request = SearchRequest()
+    search_request.index='test'
+    search_request.fullltext_filter=QueryFilter('Title 1') 
+    
+    # The example passes only required values which don't have defaults set
+    try:
+        # Perform a search
+        api_response = api_instance.search(search_request)
+        pprint(api_response)
+    except manticoresearch.ApiException as e:
+        print("Exception when calling SearchApi->search: %s\n" % e)
 ```
 
 # Documentation
 
 
-Full documentation is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder.
+Full documentation on the API Endpoints and Models used is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder as listed below.
 
 Manticore Search server documentation: https://manual.manticoresearch.com.
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://127.0.0.1:9308*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*IndexApi* | [**bulk**](docs/IndexApi.md#bulk) | **POST** /json/bulk | Bulk index operations
-*IndexApi* | [**delete**](docs/IndexApi.md#delete) | **POST** /json/delete | Delete a document in an index
-*IndexApi* | [**insert**](docs/IndexApi.md#insert) | **POST** /json/insert | Create a new document in an index
-*IndexApi* | [**replace**](docs/IndexApi.md#replace) | **POST** /json/replace | Replace new document in an index
-*IndexApi* | [**update**](docs/IndexApi.md#update) | **POST** /json/update | Update a document in an index
-*SearchApi* | [**percolate**](docs/SearchApi.md#percolate) | **POST** /json/pq/{index}/search | Perform reverse search on a percolate index
-*SearchApi* | [**search**](docs/SearchApi.md#search) | **POST** /json/search | Performs a search
+*IndexApi* | [**bulk**](docs/IndexApi.md#bulk) | **POST** /bulk | Bulk index operations
+*IndexApi* | [**delete**](docs/IndexApi.md#delete) | **POST** /delete | Delete a document in an index
+*IndexApi* | [**insert**](docs/IndexApi.md#insert) | **POST** /insert | Create a new document in an index
+*IndexApi* | [**replace**](docs/IndexApi.md#replace) | **POST** /replace | Replace new document in an index
+*IndexApi* | [**update**](docs/IndexApi.md#update) | **POST** /update | Update a document in an index
+*SearchApi* | [**percolate**](docs/SearchApi.md#percolate) | **POST** /pq/{index}/search | Perform reverse search on a percolate index
+*SearchApi* | [**search**](docs/SearchApi.md#search) | **POST** /search | Performs a search on an index
 *UtilsApi* | [**sql**](docs/UtilsApi.md#sql) | **POST** /sql | Perform SQL requests
 
 
 ## Documentation For Models
 
+ - [Aggregation](docs/Aggregation.md)
+ - [AttrFilter](docs/AttrFilter.md)
+ - [BoolFilter](docs/BoolFilter.md)
  - [BulkResponse](docs/BulkResponse.md)
  - [DeleteDocumentRequest](docs/DeleteDocumentRequest.md)
  - [DeleteResponse](docs/DeleteResponse.md)
+ - [EqualsFilter](docs/EqualsFilter.md)
  - [ErrorResponse](docs/ErrorResponse.md)
+ - [Facet](docs/Facet.md)
+ - [FilterBoolean](docs/FilterBoolean.md)
+ - [FilterNumber](docs/FilterNumber.md)
+ - [FilterString](docs/FilterString.md)
+ - [FulltextFilter](docs/FulltextFilter.md)
+ - [GeoDistanceFilter](docs/GeoDistanceFilter.md)
+ - [GeoDistanceFilterLocationAnchor](docs/GeoDistanceFilterLocationAnchor.md)
+ - [Highlight](docs/Highlight.md)
+ - [HighlightField](docs/HighlightField.md)
+ - [InFilter](docs/InFilter.md)
  - [InsertDocumentRequest](docs/InsertDocumentRequest.md)
+ - [MatchFilter](docs/MatchFilter.md)
+ - [MatchOp](docs/MatchOp.md)
+ - [MatchOpFilter](docs/MatchOpFilter.md)
+ - [MatchPhraseFilter](docs/MatchPhraseFilter.md)
+ - [NotFilterBoolean](docs/NotFilterBoolean.md)
+ - [NotFilterNumber](docs/NotFilterNumber.md)
+ - [NotFilterString](docs/NotFilterString.md)
+ - [Option](docs/Option.md)
  - [PercolateRequest](docs/PercolateRequest.md)
  - [PercolateRequestQuery](docs/PercolateRequestQuery.md)
+ - [QueryFilter](docs/QueryFilter.md)
+ - [RangeFilter](docs/RangeFilter.md)
  - [SearchRequest](docs/SearchRequest.md)
  - [SearchResponse](docs/SearchResponse.md)
  - [SearchResponseHits](docs/SearchResponseHits.md)
+ - [SortMVA](docs/SortMVA.md)
+ - [SortMultiple](docs/SortMultiple.md)
+ - [SortOrder](docs/SortOrder.md)
+ - [SourceByRules](docs/SourceByRules.md)
+ - [SourceMultiple](docs/SourceMultiple.md)
  - [SqlResponse](docs/SqlResponse.md)
  - [SuccessResponse](docs/SuccessResponse.md)
  - [UpdateDocumentRequest](docs/UpdateDocumentRequest.md)
  - [UpdateResponse](docs/UpdateResponse.md)
 
 
 ## Documentation For Authorization
```

### Comparing `manticoresearch-2.2.0/manticoresearch/api/index_api.py` & `manticoresearch-3.3.0/manticoresearch/api/index_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def bulk(self, body, **kwargs):  # noqa: E501
         """Bulk index operations  # noqa: E501
 
-        Sends multiple operatons like inserts, updates, replaces or deletes.  For each operation it's object must have same format as in their dedicated method.  The method expects a raw string as the batch in NDJSON.  Each operation object needs to be serialized to   JSON and separated by endline (\\n).      An example of raw input:      ```   {\"insert\": {\"index\": \"movies\", \"doc\": {\"plot\": \"A secret team goes to North Pole\", \"rating\": 9.5, \"language\": [2, 3], \"title\": \"This is an older movie\", \"lon\": 51.99, \"meta\": {\"keywords\":[\"travel\",\"ice\"],\"genre\":[\"adventure\"]}, \"year\": 1950, \"lat\": 60.4, \"advise\": \"PG-13\"}}}   \\n   {\"delete\": {\"index\": \"movies\",\"id\":700}}   ```      Responds with an object telling whenever any errors occured and an array with status for each operation:      ```   {'items':[{'update':{'_index':'products','_id':1,'result':'updated'}},{'update':{'_index':'products','_id':2,'result':'updated'}}],'errors':false}   ```     # noqa: E501
+        Sends multiple operatons like inserts, updates, replaces or deletes.  For each operation it's object must have same format as in their dedicated method.  The method expects a raw string as the batch in NDJSON.  Each operation object needs to be serialized to   JSON and separated by endline (\\n).      An example of raw input:      ```   {\"insert\": {\"index\": \"movies\", \"doc\": {\"plot\": \"A secret team goes to North Pole\", \"rating\": 9.5, \"language\": [2, 3], \"title\": \"This is an older movie\", \"lon\": 51.99, \"meta\": {\"keywords\":[\"travel\",\"ice\"],\"genre\":[\"adventure\"]}, \"year\": 1950, \"lat\": 60.4, \"advise\": \"PG-13\"}}}   \\n   {\"delete\": {\"index\": \"movies\",\"id\":700}}   ```      Responds with an object telling whenever any errors occured and an array with status for each operation:      ```   {     'items':     [       {         'update':{'_index':'products','_id':1,'result':'updated'}       },       {         'update':{'_index':'products','_id':2,'result':'updated'}       }     ],     'errors':false   }   ```     # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk(body, async_req=True)
         >>> result = thread.get()
 
         :param body: (required)
@@ -64,15 +64,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.bulk_with_http_info(body, **kwargs)  # noqa: E501
 
     def bulk_with_http_info(self, body, **kwargs):  # noqa: E501
         """Bulk index operations  # noqa: E501
 
-        Sends multiple operatons like inserts, updates, replaces or deletes.  For each operation it's object must have same format as in their dedicated method.  The method expects a raw string as the batch in NDJSON.  Each operation object needs to be serialized to   JSON and separated by endline (\\n).      An example of raw input:      ```   {\"insert\": {\"index\": \"movies\", \"doc\": {\"plot\": \"A secret team goes to North Pole\", \"rating\": 9.5, \"language\": [2, 3], \"title\": \"This is an older movie\", \"lon\": 51.99, \"meta\": {\"keywords\":[\"travel\",\"ice\"],\"genre\":[\"adventure\"]}, \"year\": 1950, \"lat\": 60.4, \"advise\": \"PG-13\"}}}   \\n   {\"delete\": {\"index\": \"movies\",\"id\":700}}   ```      Responds with an object telling whenever any errors occured and an array with status for each operation:      ```   {'items':[{'update':{'_index':'products','_id':1,'result':'updated'}},{'update':{'_index':'products','_id':2,'result':'updated'}}],'errors':false}   ```     # noqa: E501
+        Sends multiple operatons like inserts, updates, replaces or deletes.  For each operation it's object must have same format as in their dedicated method.  The method expects a raw string as the batch in NDJSON.  Each operation object needs to be serialized to   JSON and separated by endline (\\n).      An example of raw input:      ```   {\"insert\": {\"index\": \"movies\", \"doc\": {\"plot\": \"A secret team goes to North Pole\", \"rating\": 9.5, \"language\": [2, 3], \"title\": \"This is an older movie\", \"lon\": 51.99, \"meta\": {\"keywords\":[\"travel\",\"ice\"],\"genre\":[\"adventure\"]}, \"year\": 1950, \"lat\": 60.4, \"advise\": \"PG-13\"}}}   \\n   {\"delete\": {\"index\": \"movies\",\"id\":700}}   ```      Responds with an object telling whenever any errors occured and an array with status for each operation:      ```   {     'items':     [       {         'update':{'_index':'products','_id':1,'result':'updated'}       },       {         'update':{'_index':'products','_id':2,'result':'updated'}       }     ],     'errors':false   }   ```     # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.bulk_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param body: (required)
@@ -150,15 +150,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/x-ndjson'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/bulk', 'POST',
+            '/bulk', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='BulkResponse',  # noqa: E501
@@ -171,15 +171,15 @@
             _request_auth=local_var_params.get('_request_auth'))
         return res
          
 
     def delete(self, delete_document_request, **kwargs):  # noqa: E501
         """Delete a document in an index  # noqa: E501
 
-        Delete one or several documents. The method has 2 ways of deleting: either by id, in case only one document is deleted or by using a  match query, in which case multiple documents can be delete . Example of input to delete by id:    ```   {'index':'movies','id':100}   ```  Example of input to delete using a query:    ```   {'index':'movies','query':{'bool':{'must':[{'query_string':'new movie'}]}}}   ```  The match query has same syntax as in for searching. Responds with an object telling how many documents got deleted:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
+        Delete one or several documents. The method has 2 ways of deleting: either by id, in case only one document is deleted or by using a  match query, in which case multiple documents can be delete . Example of input to delete by id:    ```   {'index':'movies','id':100}   ```  Example of input to delete using a query:    ```   {     'index':'movies',     'query':     {       'bool':       {         'must':         [           {'query_string':'new movie'}         ]       }     }   }   ```  The match query has same syntax as in for searching. Responds with an object telling how many documents got deleted:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete(delete_document_request, async_req=True)
         >>> result = thread.get()
 
         :param delete_document_request: (required)
@@ -201,15 +201,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_with_http_info(delete_document_request, **kwargs)  # noqa: E501
 
     def delete_with_http_info(self, delete_document_request, **kwargs):  # noqa: E501
         """Delete a document in an index  # noqa: E501
 
-        Delete one or several documents. The method has 2 ways of deleting: either by id, in case only one document is deleted or by using a  match query, in which case multiple documents can be delete . Example of input to delete by id:    ```   {'index':'movies','id':100}   ```  Example of input to delete using a query:    ```   {'index':'movies','query':{'bool':{'must':[{'query_string':'new movie'}]}}}   ```  The match query has same syntax as in for searching. Responds with an object telling how many documents got deleted:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
+        Delete one or several documents. The method has 2 ways of deleting: either by id, in case only one document is deleted or by using a  match query, in which case multiple documents can be delete . Example of input to delete by id:    ```   {'index':'movies','id':100}   ```  Example of input to delete using a query:    ```   {     'index':'movies',     'query':     {       'bool':       {         'must':         [           {'query_string':'new movie'}         ]       }     }   }   ```  The match query has same syntax as in for searching. Responds with an object telling how many documents got deleted:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_with_http_info(delete_document_request, async_req=True)
         >>> result = thread.get()
 
         :param delete_document_request: (required)
@@ -287,15 +287,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/delete', 'POST',
+            '/delete', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='DeleteResponse',  # noqa: E501
@@ -308,15 +308,15 @@
             _request_auth=local_var_params.get('_request_auth'))
         return res
          
 
     def insert(self, insert_document_request, **kwargs):  # noqa: E501
         """Create a new document in an index  # noqa: E501
 
-        Insert a document.  Expects an object like:     ```   {'index':'movies','id':701,'doc':{'title':'This is an old movie','plot':'A secret team goes to North Pole','year':1950,'rating':9.5,'lat':60.4,'lon':51.99,'advise':'PG-13','meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}','language':[2,3]}}   ```   The document id can also be missing, in which case an autogenerated one will be used:             ```   {'index':'movies','doc':{'title':'This is a new movie','plot':'A secret team goes to North Pole','year':2020,'rating':9.5,'lat':60.4,'lon':51.99,'advise':'PG-13','meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}','language':[2,3]}}   ```   It responds with an object in format:      ```   {'_index':'products','_id':701,'created':true,'result':'created','status':201}   ```   # noqa: E501
+        Insert a document.  Expects an object like:     ```   {     'index':'movies',     'id':701,     'doc':     {       'title':'This is an old movie',       'plot':'A secret team goes to North Pole',       'year':1950,       'rating':9.5,       'lat':60.4,       'lon':51.99,       'advise':'PG-13',       'meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}',       'language':[2,3]     }   }   ```   The document id can also be missing, in which case an autogenerated one will be used:             ```   {     'index':'movies',     'doc':     {       'title':'This is a new movie',       'plot':'A secret team goes to North Pole',       'year':2020,       'rating':9.5,       'lat':60.4,       'lon':51.99,       'advise':'PG-13',       'meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}',       'language':[2,3]     }   }   ```   It responds with an object in format:      ```   {'_index':'products','_id':701,'created':true,'result':'created','status':201}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.insert(insert_document_request, async_req=True)
         >>> result = thread.get()
 
         :param insert_document_request: (required)
@@ -338,15 +338,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.insert_with_http_info(insert_document_request, **kwargs)  # noqa: E501
 
     def insert_with_http_info(self, insert_document_request, **kwargs):  # noqa: E501
         """Create a new document in an index  # noqa: E501
 
-        Insert a document.  Expects an object like:     ```   {'index':'movies','id':701,'doc':{'title':'This is an old movie','plot':'A secret team goes to North Pole','year':1950,'rating':9.5,'lat':60.4,'lon':51.99,'advise':'PG-13','meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}','language':[2,3]}}   ```   The document id can also be missing, in which case an autogenerated one will be used:             ```   {'index':'movies','doc':{'title':'This is a new movie','plot':'A secret team goes to North Pole','year':2020,'rating':9.5,'lat':60.4,'lon':51.99,'advise':'PG-13','meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}','language':[2,3]}}   ```   It responds with an object in format:      ```   {'_index':'products','_id':701,'created':true,'result':'created','status':201}   ```   # noqa: E501
+        Insert a document.  Expects an object like:     ```   {     'index':'movies',     'id':701,     'doc':     {       'title':'This is an old movie',       'plot':'A secret team goes to North Pole',       'year':1950,       'rating':9.5,       'lat':60.4,       'lon':51.99,       'advise':'PG-13',       'meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}',       'language':[2,3]     }   }   ```   The document id can also be missing, in which case an autogenerated one will be used:             ```   {     'index':'movies',     'doc':     {       'title':'This is a new movie',       'plot':'A secret team goes to North Pole',       'year':2020,       'rating':9.5,       'lat':60.4,       'lon':51.99,       'advise':'PG-13',       'meta':'{\"keywords\":{\"travel\",\"ice\"},\"genre\":{\"adventure\"}}',       'language':[2,3]     }   }   ```   It responds with an object in format:      ```   {'_index':'products','_id':701,'created':true,'result':'created','status':201}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.insert_with_http_info(insert_document_request, async_req=True)
         >>> result = thread.get()
 
         :param insert_document_request: (required)
@@ -424,15 +424,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/insert', 'POST',
+            '/insert', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SuccessResponse',  # noqa: E501
@@ -561,15 +561,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/replace', 'POST',
+            '/replace', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SuccessResponse',  # noqa: E501
@@ -582,15 +582,15 @@
             _request_auth=local_var_params.get('_request_auth'))
         return res
          
 
     def update(self, update_document_request, **kwargs):  # noqa: E501
         """Update a document in an index  # noqa: E501
 
-        Update one or several documents. The update can be made by passing the id or by using a match query in case multiple documents can be updated.  For example update a document using document id:    ```   {'index':'movies','doc':{'rating':9.49},'id':100}   ```  And update by using a match query:    ```   {'index':'movies','doc':{'rating':9.49},'query':{'bool':{'must':[{'query_string':'new movie'}]}}}   ```   The match query has same syntax as for searching. Responds with an object that tells how many documents where updated in format:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
+        Update one or several documents. The update can be made by passing the id or by using a match query in case multiple documents can be updated.  For example update a document using document id:    ```   {'index':'movies','doc':{'rating':9.49},'id':100}   ```  And update by using a match query:    ```   {     'index':'movies',     'doc':{'rating':9.49},     'query':     {       'bool':       {         'must':         [           {'query_string':'new movie'}         ]       }     }   }   ```   The match query has same syntax as for searching. Responds with an object that tells how many documents where updated in format:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update(update_document_request, async_req=True)
         >>> result = thread.get()
 
         :param update_document_request: (required)
@@ -612,15 +612,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.update_with_http_info(update_document_request, **kwargs)  # noqa: E501
 
     def update_with_http_info(self, update_document_request, **kwargs):  # noqa: E501
         """Update a document in an index  # noqa: E501
 
-        Update one or several documents. The update can be made by passing the id or by using a match query in case multiple documents can be updated.  For example update a document using document id:    ```   {'index':'movies','doc':{'rating':9.49},'id':100}   ```  And update by using a match query:    ```   {'index':'movies','doc':{'rating':9.49},'query':{'bool':{'must':[{'query_string':'new movie'}]}}}   ```   The match query has same syntax as for searching. Responds with an object that tells how many documents where updated in format:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
+        Update one or several documents. The update can be made by passing the id or by using a match query in case multiple documents can be updated.  For example update a document using document id:    ```   {'index':'movies','doc':{'rating':9.49},'id':100}   ```  And update by using a match query:    ```   {     'index':'movies',     'doc':{'rating':9.49},     'query':     {       'bool':       {         'must':         [           {'query_string':'new movie'}         ]       }     }   }   ```   The match query has same syntax as for searching. Responds with an object that tells how many documents where updated in format:     ```   {'_index':'products','updated':1}   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_with_http_info(update_document_request, async_req=True)
         >>> result = thread.get()
 
         :param update_document_request: (required)
@@ -698,15 +698,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/update', 'POST',
+            '/update', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='UpdateResponse',  # noqa: E501
```

### Comparing `manticoresearch-2.2.0/manticoresearch/api/search_api.py` & `manticoresearch-3.3.0/manticoresearch/api/search_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def percolate(self, index, percolate_request, **kwargs):  # noqa: E501
         """Perform reverse search on a percolate index  # noqa: E501
 
-        Performs a percolate search.  This method must be used only on percolate indexes.  Expects two parameters: the index name and an object with array of documents to be tested. An example of the documents object:    ```   {\"query\":{\"percolate\":{\"document\":{\"content\":\"sample content\"}}}}   ```  Responds with an object with matched stored queries:     ```   {'timed_out':false,'hits':{'total':2,'max_score':1,'hits':[{'_index':'idx_pq_1','_type':'doc','_id':'2','_score':'1','_source':{'query':{'match':{'title':'some'},}}},{'_index':'idx_pq_1','_type':'doc','_id':'5','_score':'1','_source':{'query':{'ql':'some | none'}}}]}}   ```   # noqa: E501
+        Performs a percolate search.  This method must be used only on percolate indexes.  Expects two parameters: the index name and an object with array of documents to be tested. An example of the documents object:    ```   {     \"query\":     {       \"percolate\":       {         \"document\":         {           \"content\":\"sample content\"         }       }     }   }   ```  Responds with an object with matched stored queries:     ```   {     'timed_out':false,     'hits':     {       'total':2,       'max_score':1,       'hits':       [         {           '_index':'idx_pq_1',           '_type':'doc',           '_id':'2',           '_score':'1',           '_source':           {             'query':             {               'match':{'title':'some'}             }           }         },         {           '_index':'idx_pq_1',           '_type':'doc',           '_id':'5',           '_score':'1',           '_source':           {             'query':             {               'ql':'some | none'             }           }         }       ]     }   }   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.percolate(index, percolate_request, async_req=True)
         >>> result = thread.get()
 
         :param index: Name of the percolate index (required)
@@ -66,15 +66,15 @@
         """
         kwargs['_return_http_data_only'] = True
         return self.percolate_with_http_info(index, percolate_request, **kwargs)  # noqa: E501
 
     def percolate_with_http_info(self, index, percolate_request, **kwargs):  # noqa: E501
         """Perform reverse search on a percolate index  # noqa: E501
 
-        Performs a percolate search.  This method must be used only on percolate indexes.  Expects two parameters: the index name and an object with array of documents to be tested. An example of the documents object:    ```   {\"query\":{\"percolate\":{\"document\":{\"content\":\"sample content\"}}}}   ```  Responds with an object with matched stored queries:     ```   {'timed_out':false,'hits':{'total':2,'max_score':1,'hits':[{'_index':'idx_pq_1','_type':'doc','_id':'2','_score':'1','_source':{'query':{'match':{'title':'some'},}}},{'_index':'idx_pq_1','_type':'doc','_id':'5','_score':'1','_source':{'query':{'ql':'some | none'}}}]}}   ```   # noqa: E501
+        Performs a percolate search.  This method must be used only on percolate indexes.  Expects two parameters: the index name and an object with array of documents to be tested. An example of the documents object:    ```   {     \"query\":     {       \"percolate\":       {         \"document\":         {           \"content\":\"sample content\"         }       }     }   }   ```  Responds with an object with matched stored queries:     ```   {     'timed_out':false,     'hits':     {       'total':2,       'max_score':1,       'hits':       [         {           '_index':'idx_pq_1',           '_type':'doc',           '_id':'2',           '_score':'1',           '_source':           {             'query':             {               'match':{'title':'some'}             }           }         },         {           '_index':'idx_pq_1',           '_type':'doc',           '_id':'5',           '_score':'1',           '_source':           {             'query':             {               'ql':'some | none'             }           }         }       ]     }   }   ```   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.percolate_with_http_info(index, percolate_request, async_req=True)
         >>> result = thread.get()
 
         :param index: Name of the percolate index (required)
@@ -161,15 +161,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/pq/{index}/search', 'POST',
+            '/pq/{index}/search', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SearchResponse',  # noqa: E501
@@ -180,17 +180,17 @@
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
         return res
          
 
     def search(self, search_request, **kwargs):  # noqa: E501
-        """Performs a search  # noqa: E501
+        """Performs a search on an index  # noqa: E501
 
-         Expects an object with mandatory properties: * the index name * the match query object Example :    ```   {'index':'movies','query':{'bool':{'must':[{'query_string':' movie'}]}},'script_fields':{'myexpr':{'script':{'inline':'IF(rating>8,1,0)'}}},'sort':[{'myexpr':'desc'},{'_score':'desc'}],'profile':true}   ```  It responds with an object with: - time of execution - if the query timed out - an array with hits (matched documents) - additional, if profiling is enabled, an array with profiling information is attached     ```   {'took':10,'timed_out':false,'hits':{'total':2,'hits':[{'_id':'1','_score':1,'_source':{'gid':11}},{'_id':'2','_score':1,'_source':{'gid':12}}]}}   ```  For more information about the match query syntax, additional paramaters that can be set to the input and response, please check: https://manual.manticoresearch.com/Searching/Full_text_matching/Basic_usage#HTTP.   # noqa: E501
+         The method expects an object with the following mandatory properties: * the name of the index to search * the match query object For details, see the documentation on [**SearchRequest**](SearchRequest.md) The method returns an object with the following properties: - took: the time taken to execute the search query. - timed_out: a boolean indicating whether the query timed out. - hits: an object with the following properties:    - total: the total number of hits found.    - hits: an array of hit objects, where each hit object represents a matched document. Each hit object has the following properties:      - _id: the ID of the matched document.      - _score: the score of the matched document.      - _source: the source data of the matched document.  In addition, if profiling is enabled, the response will include an additional array with profiling information attached. Here is an example search response:    ```   {     'took':10,     'timed_out':false,     'hits':     {       'total':2,       'hits':       [         {'_id':'1','_score':1,'_source':{'gid':11}},         {'_id':'2','_score':1,'_source':{'gid':12}}       ]     }   }   ```  For more information about the match query syntax and additional parameters that can be added to request and response, please see the documentation [here](https://manual.manticoresearch.com/Searching/Full_text_matching/Basic_usage#HTTP-JSON).   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.search(search_request, async_req=True)
         >>> result = thread.get()
 
         :param search_request: (required)
@@ -210,17 +210,17 @@
                  returns the request thread.
         :rtype: SearchResponse
         """
         kwargs['_return_http_data_only'] = True
         return self.search_with_http_info(search_request, **kwargs)  # noqa: E501
 
     def search_with_http_info(self, search_request, **kwargs):  # noqa: E501
-        """Performs a search  # noqa: E501
+        """Performs a search on an index  # noqa: E501
 
-         Expects an object with mandatory properties: * the index name * the match query object Example :    ```   {'index':'movies','query':{'bool':{'must':[{'query_string':' movie'}]}},'script_fields':{'myexpr':{'script':{'inline':'IF(rating>8,1,0)'}}},'sort':[{'myexpr':'desc'},{'_score':'desc'}],'profile':true}   ```  It responds with an object with: - time of execution - if the query timed out - an array with hits (matched documents) - additional, if profiling is enabled, an array with profiling information is attached     ```   {'took':10,'timed_out':false,'hits':{'total':2,'hits':[{'_id':'1','_score':1,'_source':{'gid':11}},{'_id':'2','_score':1,'_source':{'gid':12}}]}}   ```  For more information about the match query syntax, additional paramaters that can be set to the input and response, please check: https://manual.manticoresearch.com/Searching/Full_text_matching/Basic_usage#HTTP.   # noqa: E501
+         The method expects an object with the following mandatory properties: * the name of the index to search * the match query object For details, see the documentation on [**SearchRequest**](SearchRequest.md) The method returns an object with the following properties: - took: the time taken to execute the search query. - timed_out: a boolean indicating whether the query timed out. - hits: an object with the following properties:    - total: the total number of hits found.    - hits: an array of hit objects, where each hit object represents a matched document. Each hit object has the following properties:      - _id: the ID of the matched document.      - _score: the score of the matched document.      - _source: the source data of the matched document.  In addition, if profiling is enabled, the response will include an additional array with profiling information attached. Here is an example search response:    ```   {     'took':10,     'timed_out':false,     'hits':     {       'total':2,       'hits':       [         {'_id':'1','_score':1,'_source':{'gid':11}},         {'_id':'2','_score':1,'_source':{'gid':12}}       ]     }   }   ```  For more information about the match query syntax and additional parameters that can be added to request and response, please see the documentation [here](https://manual.manticoresearch.com/Searching/Full_text_matching/Basic_usage#HTTP-JSON).   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.search_with_http_info(search_request, async_req=True)
         >>> result = thread.get()
 
         :param search_request: (required)
@@ -285,28 +285,31 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         if 'search_request' in local_var_params:
             body_params = local_var_params['search_request']
+            if type(body_params) != dict:
+                body_params = body_params.to_dict()
+            body_params = dict(filter(lambda item: item[1] is not None, body_params.items() )) 
 
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = []  # noqa: E501
 
         res = self.api_client.call_api(
-            '/json/search', 'POST',
+            '/search', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='SearchResponse',  # noqa: E501
```

### Comparing `manticoresearch-2.2.0/manticoresearch/api/utils_api.py` & `manticoresearch-3.3.0/manticoresearch/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/manticoresearch/api_client.py` & `manticoresearch-3.3.0/manticoresearch/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'manticoresearch/2.2.0/python'
+        self.user_agent = 'manticoresearch/3.3.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `manticoresearch-2.2.0/manticoresearch/apis/__init__.py` & `manticoresearch-3.3.0/manticoresearch/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/manticoresearch/configuration.py` & `manticoresearch-3.3.0/manticoresearch/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,16 +367,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 2.2.0".\
+               "Version of the API: 3.3.0\n"\
+               "SDK Package Version: 3.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `manticoresearch-2.2.0/manticoresearch/exceptions.py` & `manticoresearch-3.3.0/manticoresearch/exceptions.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/manticoresearch/model/bulk_response.py` & `manticoresearch-3.3.0/manticoresearch/model/bulk_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class BulkResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -60,51 +59,52 @@
         """Gets the items of this BulkResponse.  # noqa: E501
 
 
         :return: The items of this BulkResponse.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._items
-
     @items.setter
     def items(self, items):
         """Sets the items of this BulkResponse.
 
 
         :param items: The items of this BulkResponse.  # noqa: E501
         :type items: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._items = items
+        
 
     @property
     def error(self):
         """Gets the error of this BulkResponse.  # noqa: E501
 
 
         :return: The error of this BulkResponse.  # noqa: E501
         :rtype: bool
         """
         return self._error
-
     @error.setter
     def error(self, error):
         """Sets the error of this BulkResponse.
 
 
         :param error: The error of this BulkResponse.  # noqa: E501
         :type error: bool
         """
 
         self._error = error
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -115,14 +115,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/delete_document_request.py` & `manticoresearch-3.3.0/manticoresearch/model/delete_document_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class DeleteDocumentRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -70,102 +69,103 @@
 
         Index name  # noqa: E501
 
         :return: The index of this DeleteDocumentRequest.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this DeleteDocumentRequest.
 
         Index name  # noqa: E501
 
         :param index: The index of this DeleteDocumentRequest.  # noqa: E501
         :type index: str
         """
         if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
             raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
 
         self._index = index
+        
 
     @property
     def cluster(self):
         """Gets the cluster of this DeleteDocumentRequest.  # noqa: E501
 
         cluster name  # noqa: E501
 
         :return: The cluster of this DeleteDocumentRequest.  # noqa: E501
         :rtype: str
         """
         return self._cluster
-
     @cluster.setter
     def cluster(self, cluster):
         """Sets the cluster of this DeleteDocumentRequest.
 
         cluster name  # noqa: E501
 
         :param cluster: The cluster of this DeleteDocumentRequest.  # noqa: E501
         :type cluster: str
         """
 
         self._cluster = cluster
+        
 
     @property
     def id(self):
         """Gets the id of this DeleteDocumentRequest.  # noqa: E501
 
         Document ID  # noqa: E501
 
         :return: The id of this DeleteDocumentRequest.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this DeleteDocumentRequest.
 
         Document ID  # noqa: E501
 
         :param id: The id of this DeleteDocumentRequest.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def query(self):
         """Gets the query of this DeleteDocumentRequest.  # noqa: E501
 
         Query tree object  # noqa: E501
 
         :return: The query of this DeleteDocumentRequest.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._query
-
     @query.setter
     def query(self, query):
         """Sets the query of this DeleteDocumentRequest.
 
         Query tree object  # noqa: E501
 
         :param query: The query of this DeleteDocumentRequest.  # noqa: E501
         :type query: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._query = query
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -176,14 +176,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/delete_response.py` & `manticoresearch-3.3.0/manticoresearch/model/delete_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class DeleteResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -70,93 +69,94 @@
         """Gets the index of this DeleteResponse.  # noqa: E501
 
 
         :return: The index of this DeleteResponse.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this DeleteResponse.
 
 
         :param index: The index of this DeleteResponse.  # noqa: E501
         :type index: str
         """
 
         self._index = index
+        
 
     @property
     def deleted(self):
         """Gets the deleted of this DeleteResponse.  # noqa: E501
 
 
         :return: The deleted of this DeleteResponse.  # noqa: E501
         :rtype: int
         """
         return self._deleted
-
     @deleted.setter
     def deleted(self, deleted):
         """Sets the deleted of this DeleteResponse.
 
 
         :param deleted: The deleted of this DeleteResponse.  # noqa: E501
         :type deleted: int
         """
 
         self._deleted = deleted
+        
 
     @property
     def id(self):
         """Gets the id of this DeleteResponse.  # noqa: E501
 
 
         :return: The id of this DeleteResponse.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this DeleteResponse.
 
 
         :param id: The id of this DeleteResponse.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def result(self):
         """Gets the result of this DeleteResponse.  # noqa: E501
 
 
         :return: The result of this DeleteResponse.  # noqa: E501
         :rtype: str
         """
         return self._result
-
     @result.setter
     def result(self, result):
         """Sets the result of this DeleteResponse.
 
 
         :param result: The result of this DeleteResponse.  # noqa: E501
         :type result: str
         """
 
         self._result = result
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -167,14 +167,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/error_response.py` & `manticoresearch-3.3.0/manticoresearch/model/error_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class ErrorResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -58,55 +57,56 @@
         """Gets the error of this ErrorResponse.  # noqa: E501
 
 
         :return: The error of this ErrorResponse.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._error
-
     @error.setter
     def error(self, error):
         """Sets the error of this ErrorResponse.
 
 
         :param error: The error of this ErrorResponse.  # noqa: E501
         :type error: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         if self.local_vars_configuration.client_side_validation and error is None:  # noqa: E501
             raise ValueError("Invalid value for `error`, must not be `None`")  # noqa: E501
 
         self._error = error
+        
 
     @property
     def status(self):
         """Gets the status of this ErrorResponse.  # noqa: E501
 
 
         :return: The status of this ErrorResponse.  # noqa: E501
         :rtype: int
         """
         return self._status
-
     @status.setter
     def status(self, status):
         """Sets the status of this ErrorResponse.
 
 
         :param status: The status of this ErrorResponse.  # noqa: E501
         :type status: int
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
 
         self._status = status
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -117,14 +117,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/insert_document_request.py` & `manticoresearch-3.3.0/manticoresearch/model/insert_document_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class InsertDocumentRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -69,104 +68,105 @@
 
         Name of the index  # noqa: E501
 
         :return: The index of this InsertDocumentRequest.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this InsertDocumentRequest.
 
         Name of the index  # noqa: E501
 
         :param index: The index of this InsertDocumentRequest.  # noqa: E501
         :type index: str
         """
         if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
             raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
 
         self._index = index
+        
 
     @property
     def cluster(self):
         """Gets the cluster of this InsertDocumentRequest.  # noqa: E501
 
         cluster name  # noqa: E501
 
         :return: The cluster of this InsertDocumentRequest.  # noqa: E501
         :rtype: str
         """
         return self._cluster
-
     @cluster.setter
     def cluster(self, cluster):
         """Sets the cluster of this InsertDocumentRequest.
 
         cluster name  # noqa: E501
 
         :param cluster: The cluster of this InsertDocumentRequest.  # noqa: E501
         :type cluster: str
         """
 
         self._cluster = cluster
+        
 
     @property
     def id(self):
         """Gets the id of this InsertDocumentRequest.  # noqa: E501
 
         Document ID.   # noqa: E501
 
         :return: The id of this InsertDocumentRequest.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this InsertDocumentRequest.
 
         Document ID.   # noqa: E501
 
         :param id: The id of this InsertDocumentRequest.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def doc(self):
         """Gets the doc of this InsertDocumentRequest.  # noqa: E501
 
         Object with document data   # noqa: E501
 
         :return: The doc of this InsertDocumentRequest.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._doc
-
     @doc.setter
     def doc(self, doc):
         """Sets the doc of this InsertDocumentRequest.
 
         Object with document data   # noqa: E501
 
         :param doc: The doc of this InsertDocumentRequest.  # noqa: E501
         :type doc: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         if self.local_vars_configuration.client_side_validation and doc is None:  # noqa: E501
             raise ValueError("Invalid value for `doc`, must not be `None`")  # noqa: E501
 
         self._doc = doc
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -177,14 +177,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/percolate_request.py` & `manticoresearch-3.3.0/manticoresearch/model/percolate_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class PercolateRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -54,32 +53,33 @@
         """Gets the query of this PercolateRequest.  # noqa: E501
 
 
         :return: The query of this PercolateRequest.  # noqa: E501
         :rtype: PercolateRequestQuery
         """
         return self._query
-
     @query.setter
     def query(self, query):
         """Sets the query of this PercolateRequest.
 
 
         :param query: The query of this PercolateRequest.  # noqa: E501
         :type query: PercolateRequestQuery
         """
         if self.local_vars_configuration.client_side_validation and query is None:  # noqa: E501
             raise ValueError("Invalid value for `query`, must not be `None`")  # noqa: E501
 
         self._query = query
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -90,14 +90,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/percolate_request_query.py` & `manticoresearch-3.3.0/manticoresearch/model/percolate_request_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class PercolateRequestQuery(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -54,32 +53,33 @@
         """Gets the percolate of this PercolateRequestQuery.  # noqa: E501
 
 
         :return: The percolate of this PercolateRequestQuery.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._percolate
-
     @percolate.setter
     def percolate(self, percolate):
         """Sets the percolate of this PercolateRequestQuery.
 
 
         :param percolate: The percolate of this PercolateRequestQuery.  # noqa: E501
         :type percolate: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         if self.local_vars_configuration.client_side_validation and percolate is None:  # noqa: E501
             raise ValueError("Invalid value for `percolate`, must not be `None`")  # noqa: E501
 
         self._percolate = percolate
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -90,14 +90,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/search_request.py` & `manticoresearch-3.3.0/manticoresearch/model/search_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class SearchRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -29,63 +28,77 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'index': 'str',
         'query': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
+        'fulltext_filter': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
+        'attr_filter': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
         'limit': 'int',
         'offset': 'int',
         'max_matches': 'int',
         'sort': '[{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]',
-        'aggs': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'expressions': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'highlight': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'source': '[str]',
+        'aggs': '[Aggregation]',
+        'expressions': '[{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]',
+        'highlight': 'Highlight',
+        'source': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
         'options': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
-        'profile': 'bool'
+        'profile': 'bool',
+        'track_scores': 'bool'
     }
 
     attribute_map = {
         'index': 'index',
         'query': 'query',
+        'fulltext_filter': 'fulltext_filter',
+        'attr_filter': 'attr_filter',
         'limit': 'limit',
         'offset': 'offset',
         'max_matches': 'max_matches',
         'sort': 'sort',
         'aggs': 'aggs',
         'expressions': 'expressions',
         'highlight': 'highlight',
-        'source': '_source',
+        'source': 'source',
         'options': 'options',
-        'profile': 'profile'
+        'profile': 'profile',
+        'track_scores': 'track_scores'
     }
 
-    def __init__(self, index=None, query=None, limit=None, offset=None, max_matches=None, sort=None, aggs=None, expressions=None, highlight=None, source=None, options=None, profile=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, index="", query=None, fulltext_filter=None, attr_filter=None, limit=None, offset=None, max_matches=None, sort=None, aggs=None, expressions=None, highlight=None, source=None, options=None, profile=None, track_scores=None, local_vars_configuration=None):  # noqa: E501
         """SearchRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._index = None
         self._query = None
+        self._fulltext_filter = None
+        self._attr_filter = None
         self._limit = None
         self._offset = None
         self._max_matches = None
         self._sort = None
         self._aggs = None
         self._expressions = None
         self._highlight = None
         self._source = None
         self._options = None
         self._profile = None
+        self._track_scores = None
         self.discriminator = None
 
         self.index = index
-        self.query = query
+        if query is not None:
+            self.query = query
+        if fulltext_filter is not None:
+            self.fulltext_filter = fulltext_filter
+        if attr_filter is not None:
+            self.attr_filter = attr_filter
         if limit is not None:
             self.limit = limit
         if offset is not None:
             self.offset = offset
         if max_matches is not None:
             self.max_matches = max_matches
         if sort is not None:
@@ -98,275 +111,343 @@
             self.highlight = highlight
         if source is not None:
             self.source = source
         if options is not None:
             self.options = options
         if profile is not None:
             self.profile = profile
+        if track_scores is not None:
+            self.track_scores = track_scores
 
     @property
     def index(self):
         """Gets the index of this SearchRequest.  # noqa: E501
 
 
         :return: The index of this SearchRequest.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this SearchRequest.
 
 
         :param index: The index of this SearchRequest.  # noqa: E501
         :type index: str
         """
         if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
             raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
 
         self._index = index
+        
 
     @property
     def query(self):
         """Gets the query of this SearchRequest.  # noqa: E501
 
 
         :return: The query of this SearchRequest.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._query
-
     @query.setter
     def query(self, query):
         """Sets the query of this SearchRequest.
 
 
         :param query: The query of this SearchRequest.  # noqa: E501
         :type query: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
-        if self.local_vars_configuration.client_side_validation and query is None:  # noqa: E501
-            raise ValueError("Invalid value for `query`, must not be `None`")  # noqa: E501
 
         self._query = query
+        
+        if self.fulltext_filter is not None:
+        	self.fulltext_filter = None;
+       	if self.attr_filter is not None:
+        	self.attr_filter = None;
+
+    @property
+    def fulltext_filter(self):
+        """Gets the fulltext_filter of this SearchRequest.  # noqa: E501
+
+
+        :return: The fulltext_filter of this SearchRequest.  # noqa: E501
+        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        """
+        return self._fulltext_filter
+    @fulltext_filter.setter
+    def fulltext_filter(self, fulltext_filter):
+        """Sets the fulltext_filter of this SearchRequest.
+
+
+        :param fulltext_filter: The fulltext_filter of this SearchRequest.  # noqa: E501
+        :type fulltext_filter: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        """
+
+        self._fulltext_filter = fulltext_filter
+        
+
+    @property
+    def attr_filter(self):
+        """Gets the attr_filter of this SearchRequest.  # noqa: E501
+
+
+        :return: The attr_filter of this SearchRequest.  # noqa: E501
+        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        """
+        return self._attr_filter
+    @attr_filter.setter
+    def attr_filter(self, attr_filter):
+        """Sets the attr_filter of this SearchRequest.
+
+
+        :param attr_filter: The attr_filter of this SearchRequest.  # noqa: E501
+        :type attr_filter: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        """
+
+        self._attr_filter = attr_filter
+        
 
     @property
     def limit(self):
         """Gets the limit of this SearchRequest.  # noqa: E501
 
 
         :return: The limit of this SearchRequest.  # noqa: E501
         :rtype: int
         """
         return self._limit
-
     @limit.setter
     def limit(self, limit):
         """Sets the limit of this SearchRequest.
 
 
         :param limit: The limit of this SearchRequest.  # noqa: E501
         :type limit: int
         """
 
         self._limit = limit
+        
 
     @property
     def offset(self):
         """Gets the offset of this SearchRequest.  # noqa: E501
 
 
         :return: The offset of this SearchRequest.  # noqa: E501
         :rtype: int
         """
         return self._offset
-
     @offset.setter
     def offset(self, offset):
         """Sets the offset of this SearchRequest.
 
 
         :param offset: The offset of this SearchRequest.  # noqa: E501
         :type offset: int
         """
 
         self._offset = offset
+        
 
     @property
     def max_matches(self):
         """Gets the max_matches of this SearchRequest.  # noqa: E501
 
 
         :return: The max_matches of this SearchRequest.  # noqa: E501
         :rtype: int
         """
         return self._max_matches
-
     @max_matches.setter
     def max_matches(self, max_matches):
         """Sets the max_matches of this SearchRequest.
 
 
         :param max_matches: The max_matches of this SearchRequest.  # noqa: E501
         :type max_matches: int
         """
 
         self._max_matches = max_matches
+        
 
     @property
     def sort(self):
         """Gets the sort of this SearchRequest.  # noqa: E501
 
 
         :return: The sort of this SearchRequest.  # noqa: E501
         :rtype: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
         return self._sort
-
     @sort.setter
     def sort(self, sort):
         """Sets the sort of this SearchRequest.
 
 
         :param sort: The sort of this SearchRequest.  # noqa: E501
         :type sort: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
 
         self._sort = sort
+        
 
     @property
     def aggs(self):
         """Gets the aggs of this SearchRequest.  # noqa: E501
 
 
         :return: The aggs of this SearchRequest.  # noqa: E501
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :rtype: [Aggregation]
         """
         return self._aggs
-
     @aggs.setter
     def aggs(self, aggs):
         """Sets the aggs of this SearchRequest.
 
 
         :param aggs: The aggs of this SearchRequest.  # noqa: E501
-        :type aggs: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :type aggs: [Aggregation]
         """
 
         self._aggs = aggs
+        
 
     @property
     def expressions(self):
         """Gets the expressions of this SearchRequest.  # noqa: E501
 
 
         :return: The expressions of this SearchRequest.  # noqa: E501
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :rtype: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
         return self._expressions
-
     @expressions.setter
     def expressions(self, expressions):
         """Sets the expressions of this SearchRequest.
 
 
         :param expressions: The expressions of this SearchRequest.  # noqa: E501
-        :type expressions: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :type expressions: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
 
         self._expressions = expressions
+        
 
     @property
     def highlight(self):
         """Gets the highlight of this SearchRequest.  # noqa: E501
 
 
         :return: The highlight of this SearchRequest.  # noqa: E501
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :rtype: Highlight
         """
         return self._highlight
-
     @highlight.setter
     def highlight(self, highlight):
         """Sets the highlight of this SearchRequest.
 
 
         :param highlight: The highlight of this SearchRequest.  # noqa: E501
-        :type highlight: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :type highlight: Highlight
         """
 
         self._highlight = highlight
+        
 
     @property
     def source(self):
         """Gets the source of this SearchRequest.  # noqa: E501
 
 
         :return: The source of this SearchRequest.  # noqa: E501
-        :rtype: [str]
+        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._source
-
     @source.setter
     def source(self, source):
         """Sets the source of this SearchRequest.
 
 
         :param source: The source of this SearchRequest.  # noqa: E501
-        :type source: [str]
+        :type source: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._source = source
+        
 
     @property
     def options(self):
         """Gets the options of this SearchRequest.  # noqa: E501
 
 
         :return: The options of this SearchRequest.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._options
-
     @options.setter
     def options(self, options):
         """Sets the options of this SearchRequest.
 
 
         :param options: The options of this SearchRequest.  # noqa: E501
         :type options: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._options = options
+        
 
     @property
     def profile(self):
         """Gets the profile of this SearchRequest.  # noqa: E501
 
 
         :return: The profile of this SearchRequest.  # noqa: E501
         :rtype: bool
         """
         return self._profile
-
     @profile.setter
     def profile(self, profile):
         """Sets the profile of this SearchRequest.
 
 
         :param profile: The profile of this SearchRequest.  # noqa: E501
         :type profile: bool
         """
 
         self._profile = profile
+        
+
+    @property
+    def track_scores(self):
+        """Gets the track_scores of this SearchRequest.  # noqa: E501
+
+
+        :return: The track_scores of this SearchRequest.  # noqa: E501
+        :rtype: bool
+        """
+        return self._track_scores
+    @track_scores.setter
+    def track_scores(self, track_scores):
+        """Sets the track_scores of this SearchRequest.
+
+
+        :param track_scores: The track_scores of this SearchRequest.  # noqa: E501
+        :type track_scores: bool
+        """
+
+        self._track_scores = track_scores
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -377,14 +458,40 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+        result['_source'] = result['source']
+        del result['source']
+        if result['expressions'] is not None:
+        	result['expressions'] = {k:v for i in result['expressions'] for k,v in i.items() }
+        if result['aggs'] is not None:
+        	result['aggs'] = {
+        	    i['name']: { 'terms': { 'field': i['field'], 'size': i['size'] } } for i in result['aggs']
+        	}
+        if result['highlight'] is not None:
+	        if result['highlight']['fields'] is None: 	
+	            result['highlight']['fields'] = result['highlight']['fieldnames']
+	        result['highlight']['fieldnames'] = None
+	        result['highlight'] = {k:v for k,v in result['highlight'].items() if v is not None}
+        
+        if result['fulltext_filter'] is not None or result['attr_filter'] is not None:
+            result['query'] = {}
+        if result['fulltext_filter'] is not None:
+            for k,v in result['fulltext_filter'].items():
+                result['query'][k] = v
+            del result['fulltext_filter']
+        if result['attr_filter'] is not None:
+            for k,v in result['attr_filter'].items():
+                result['query'][k] = v
+            del result['attr_filter']
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/search_response.py` & `manticoresearch-3.3.0/manticoresearch/model/search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class SearchResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -80,135 +79,136 @@
         """Gets the took of this SearchResponse.  # noqa: E501
 
 
         :return: The took of this SearchResponse.  # noqa: E501
         :rtype: int
         """
         return self._took
-
     @took.setter
     def took(self, took):
         """Sets the took of this SearchResponse.
 
 
         :param took: The took of this SearchResponse.  # noqa: E501
         :type took: int
         """
 
         self._took = took
+        
 
     @property
     def timed_out(self):
         """Gets the timed_out of this SearchResponse.  # noqa: E501
 
 
         :return: The timed_out of this SearchResponse.  # noqa: E501
         :rtype: bool
         """
         return self._timed_out
-
     @timed_out.setter
     def timed_out(self, timed_out):
         """Sets the timed_out of this SearchResponse.
 
 
         :param timed_out: The timed_out of this SearchResponse.  # noqa: E501
         :type timed_out: bool
         """
 
         self._timed_out = timed_out
+        
 
     @property
     def aggregations(self):
         """Gets the aggregations of this SearchResponse.  # noqa: E501
 
 
         :return: The aggregations of this SearchResponse.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._aggregations
-
     @aggregations.setter
     def aggregations(self, aggregations):
         """Sets the aggregations of this SearchResponse.
 
 
         :param aggregations: The aggregations of this SearchResponse.  # noqa: E501
         :type aggregations: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._aggregations = aggregations
+        
 
     @property
     def hits(self):
         """Gets the hits of this SearchResponse.  # noqa: E501
 
 
         :return: The hits of this SearchResponse.  # noqa: E501
         :rtype: SearchResponseHits
         """
         return self._hits
-
     @hits.setter
     def hits(self, hits):
         """Sets the hits of this SearchResponse.
 
 
         :param hits: The hits of this SearchResponse.  # noqa: E501
         :type hits: SearchResponseHits
         """
 
         self._hits = hits
+        
 
     @property
     def profile(self):
         """Gets the profile of this SearchResponse.  # noqa: E501
 
 
         :return: The profile of this SearchResponse.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._profile
-
     @profile.setter
     def profile(self, profile):
         """Sets the profile of this SearchResponse.
 
 
         :param profile: The profile of this SearchResponse.  # noqa: E501
         :type profile: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._profile = profile
+        
 
     @property
     def warning(self):
         """Gets the warning of this SearchResponse.  # noqa: E501
 
 
         :return: The warning of this SearchResponse.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._warning
-
     @warning.setter
     def warning(self, warning):
         """Sets the warning of this SearchResponse.
 
 
         :param warning: The warning of this SearchResponse.  # noqa: E501
         :type warning: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
 
         self._warning = warning
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -219,14 +219,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/search_response_hits.py` & `manticoresearch-3.3.0/manticoresearch/model/search_response_hits.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class SearchResponseHits(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -70,93 +69,94 @@
         """Gets the max_score of this SearchResponseHits.  # noqa: E501
 
 
         :return: The max_score of this SearchResponseHits.  # noqa: E501
         :rtype: int
         """
         return self._max_score
-
     @max_score.setter
     def max_score(self, max_score):
         """Sets the max_score of this SearchResponseHits.
 
 
         :param max_score: The max_score of this SearchResponseHits.  # noqa: E501
         :type max_score: int
         """
 
         self._max_score = max_score
+        
 
     @property
     def total(self):
         """Gets the total of this SearchResponseHits.  # noqa: E501
 
 
         :return: The total of this SearchResponseHits.  # noqa: E501
         :rtype: int
         """
         return self._total
-
     @total.setter
     def total(self, total):
         """Sets the total of this SearchResponseHits.
 
 
         :param total: The total of this SearchResponseHits.  # noqa: E501
         :type total: int
         """
 
         self._total = total
+        
 
     @property
     def total_relation(self):
         """Gets the total_relation of this SearchResponseHits.  # noqa: E501
 
 
         :return: The total_relation of this SearchResponseHits.  # noqa: E501
         :rtype: str
         """
         return self._total_relation
-
     @total_relation.setter
     def total_relation(self, total_relation):
         """Sets the total_relation of this SearchResponseHits.
 
 
         :param total_relation: The total_relation of this SearchResponseHits.  # noqa: E501
         :type total_relation: str
         """
 
         self._total_relation = total_relation
+        
 
     @property
     def hits(self):
         """Gets the hits of this SearchResponseHits.  # noqa: E501
 
 
         :return: The hits of this SearchResponseHits.  # noqa: E501
         :rtype: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
         return self._hits
-
     @hits.setter
     def hits(self, hits):
         """Sets the hits of this SearchResponseHits.
 
 
         :param hits: The hits of this SearchResponseHits.  # noqa: E501
         :type hits: [{str: (bool, date, datetime, dict, float, int, list, str, none_type)}]
         """
 
         self._hits = hits
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -167,14 +167,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/sql_response.py` & `manticoresearch-3.3.0/manticoresearch/model/sql_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class SqlResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -39,18 +38,19 @@
     def __init__(self, local_vars_configuration=None):  # noqa: E501
         """SqlResponse - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
+
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -61,14 +61,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/success_response.py` & `manticoresearch-3.3.0/manticoresearch/model/success_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class SuccessResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -75,114 +74,115 @@
         """Gets the index of this SuccessResponse.  # noqa: E501
 
 
         :return: The index of this SuccessResponse.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this SuccessResponse.
 
 
         :param index: The index of this SuccessResponse.  # noqa: E501
         :type index: str
         """
 
         self._index = index
+        
 
     @property
     def id(self):
         """Gets the id of this SuccessResponse.  # noqa: E501
 
 
         :return: The id of this SuccessResponse.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this SuccessResponse.
 
 
         :param id: The id of this SuccessResponse.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def created(self):
         """Gets the created of this SuccessResponse.  # noqa: E501
 
 
         :return: The created of this SuccessResponse.  # noqa: E501
         :rtype: bool
         """
         return self._created
-
     @created.setter
     def created(self, created):
         """Sets the created of this SuccessResponse.
 
 
         :param created: The created of this SuccessResponse.  # noqa: E501
         :type created: bool
         """
 
         self._created = created
+        
 
     @property
     def result(self):
         """Gets the result of this SuccessResponse.  # noqa: E501
 
 
         :return: The result of this SuccessResponse.  # noqa: E501
         :rtype: str
         """
         return self._result
-
     @result.setter
     def result(self, result):
         """Sets the result of this SuccessResponse.
 
 
         :param result: The result of this SuccessResponse.  # noqa: E501
         :type result: str
         """
 
         self._result = result
+        
 
     @property
     def found(self):
         """Gets the found of this SuccessResponse.  # noqa: E501
 
 
         :return: The found of this SuccessResponse.  # noqa: E501
         :rtype: bool
         """
         return self._found
-
     @found.setter
     def found(self, found):
         """Sets the found of this SuccessResponse.
 
 
         :param found: The found of this SuccessResponse.  # noqa: E501
         :type found: bool
         """
 
         self._found = found
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -193,14 +193,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/update_document_request.py` & `manticoresearch-3.3.0/manticoresearch/model/update_document_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class UpdateDocumentRequest(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -30,15 +29,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'index': 'str',
         'doc': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}',
         'id': 'int',
-        'query': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}'
+        'query': '{str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type'
     }
 
     attribute_map = {
         'index': 'index',
         'doc': 'doc',
         'id': 'id',
         'query': 'query'
@@ -56,115 +55,115 @@
         self._query = None
         self.discriminator = None
 
         self.index = index
         self.doc = doc
         if id is not None:
             self.id = id
-        if query is not None:
-            self.query = query
+        self.query = query
 
     @property
     def index(self):
         """Gets the index of this UpdateDocumentRequest.  # noqa: E501
 
 
         :return: The index of this UpdateDocumentRequest.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this UpdateDocumentRequest.
 
 
         :param index: The index of this UpdateDocumentRequest.  # noqa: E501
         :type index: str
         """
         if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
             raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
 
         self._index = index
+        
 
     @property
     def doc(self):
         """Gets the doc of this UpdateDocumentRequest.  # noqa: E501
 
         Index name  # noqa: E501
 
         :return: The doc of this UpdateDocumentRequest.  # noqa: E501
         :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         return self._doc
-
     @doc.setter
     def doc(self, doc):
         """Sets the doc of this UpdateDocumentRequest.
 
         Index name  # noqa: E501
 
         :param doc: The doc of this UpdateDocumentRequest.  # noqa: E501
         :type doc: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
         """
         if self.local_vars_configuration.client_side_validation and doc is None:  # noqa: E501
             raise ValueError("Invalid value for `doc`, must not be `None`")  # noqa: E501
 
         self._doc = doc
+        
 
     @property
     def id(self):
         """Gets the id of this UpdateDocumentRequest.  # noqa: E501
 
         Document ID  # noqa: E501
 
         :return: The id of this UpdateDocumentRequest.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this UpdateDocumentRequest.
 
         Document ID  # noqa: E501
 
         :param id: The id of this UpdateDocumentRequest.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def query(self):
         """Gets the query of this UpdateDocumentRequest.  # noqa: E501
 
         Query tree object  # noqa: E501
 
         :return: The query of this UpdateDocumentRequest.  # noqa: E501
-        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :rtype: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type
         """
         return self._query
-
     @query.setter
     def query(self, query):
         """Sets the query of this UpdateDocumentRequest.
 
         Query tree object  # noqa: E501
 
         :param query: The query of this UpdateDocumentRequest.  # noqa: E501
-        :type query: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}
+        :type query: {str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type
         """
 
         self._query = query
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -175,14 +174,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model/update_response.py` & `manticoresearch-3.3.0/manticoresearch/model/update_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from manticoresearch.configuration import Configuration
 
-
 class UpdateResponse(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -70,93 +69,94 @@
         """Gets the index of this UpdateResponse.  # noqa: E501
 
 
         :return: The index of this UpdateResponse.  # noqa: E501
         :rtype: str
         """
         return self._index
-
     @index.setter
     def index(self, index):
         """Sets the index of this UpdateResponse.
 
 
         :param index: The index of this UpdateResponse.  # noqa: E501
         :type index: str
         """
 
         self._index = index
+        
 
     @property
     def updated(self):
         """Gets the updated of this UpdateResponse.  # noqa: E501
 
 
         :return: The updated of this UpdateResponse.  # noqa: E501
         :rtype: int
         """
         return self._updated
-
     @updated.setter
     def updated(self, updated):
         """Sets the updated of this UpdateResponse.
 
 
         :param updated: The updated of this UpdateResponse.  # noqa: E501
         :type updated: int
         """
 
         self._updated = updated
+        
 
     @property
     def id(self):
         """Gets the id of this UpdateResponse.  # noqa: E501
 
 
         :return: The id of this UpdateResponse.  # noqa: E501
         :rtype: int
         """
         return self._id
-
     @id.setter
     def id(self, id):
         """Sets the id of this UpdateResponse.
 
 
         :param id: The id of this UpdateResponse.  # noqa: E501
         :type id: int
         """
 
         self._id = id
+        
 
     @property
     def result(self):
         """Gets the result of this UpdateResponse.  # noqa: E501
 
 
         :return: The result of this UpdateResponse.  # noqa: E501
         :rtype: str
         """
         return self._result
-
     @result.setter
     def result(self, result):
         """Sets the result of this UpdateResponse.
 
 
         :param result: The result of this UpdateResponse.  # noqa: E501
         :type result: str
         """
 
         self._result = result
+        
+
 
     def to_dict(self):
         """Returns the model properties as a dict"""
-        result = {}
 
+        result = {}		
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
                 result[attr] = list(map(
                     lambda x: x.to_dict() if hasattr(x, "to_dict") else x,
                     value
                 ))
@@ -167,14 +167,16 @@
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
 
+
+
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
         return pprint.pformat(self.to_dict())
 
     def __repr__(self):
```

### Comparing `manticoresearch-2.2.0/manticoresearch/model_utils.py` & `manticoresearch-3.3.0/manticoresearch/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Manticore Search Client
 
-    Low-level client for Manticore Search.   # noqa: E501
+    Сlient for Manticore Search.   # noqa: E501
 
-    The version of the OpenAPI document: 1.0.0
+    The version of the OpenAPI document: 3.3.0
     Contact: info@manticoresearch.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
@@ -202,15 +202,15 @@
 
     def __deepcopy__(self, memo):
         cls = self.__class__
 
         if self.get("_spec_property_naming", False):
             new_inst = cls._new_from_openapi_data()
         else:
-            new_inst = cls.__new__(cls)
+            new_inst = cls.__new__(cls, **self.__dict__)
 
         for k, v in self.__dict__.items():
             setattr(new_inst, k, deepcopy(v, memo))
         return new_inst
 
 
     def __new__(cls, *args, **kwargs):
@@ -2043,15 +2043,17 @@
     """
     discarded_args = get_discarded_args(self, composed_instances, model_args)
 
     # map variable names to composed_instances
     var_name_to_model_instances = {}
     for prop_name in model_args:
         if prop_name not in discarded_args:
-            var_name_to_model_instances[prop_name] = [self] + composed_instances
+            var_name_to_model_instances[prop_name] = [self] + list(
+                filter(
+                    lambda x: prop_name in x.openapi_types, composed_instances))
 
     return [
         composed_instances,
         var_name_to_model_instances,
         additional_properties_model_instances,
         discarded_args
     ]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `manticoresearch-2.2.0/manticoresearch/rest.py` & `manticoresearch-3.3.0/manticoresearch/rest.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/manticoresearch.egg-info/PKG-INFO` & `manticoresearch-3.3.0/manticoresearch.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: manticoresearch
-Version: 2.2.0
+Version: 3.3.0
 Summary: Python client for Manticore Search
-Home-page: UNKNOWN
+Home-page: 
 Author: Manticore Software Ltd.
 Author-email: info@manticoresearch.com
 License: MIT
 Project-URL: Documentation, https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs
 Project-URL: Source Code, https://github.com/manticoresoftware/manticoresearch-python
 Project-URL: Issue Tracker, https://github.com/manticoresoftware/manticoresearch-python/issues
 Keywords: full-text search,manticoresearch,search
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -26,30 +25,27 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # manticoresearch
-Low-level client for Manticore Search.
+Сlient for Manticore Search.
 
 
-❗ WARNING: this is a development version of the client. The latest release's readme is https://github.com/manticoresoftware/manticoresearch-python/tree/2.2.0
 
 ## Requirements.
 
-Python 2.7 and 3.4+.
-
-Minimum Manticore Search version is > 2.5.1 with HTTP protocol enabled.
+Minimum Manticore Search version is >= 2.5.1 with HTTP protocol enabled.
 
 | Manticore Search  | manticoresearch-python   |     Python    |
 | ----------------- | ------------------------ | ------------- |
 | >= 4.2.1          | 2.0.x                    | >= 3.4        |
-| >= 4.0.2          | 1.0.6                    | >= 3.4        |
-| >= 2.5.1          | 1.0.5                    | >= 2.7        |
+| >= 4.0.2  < 4.2.1 | 1.0.6                    | >= 3.4        |
+| >= 2.5.1  < 4.0.2 | 1.0.5                    | >= 2.7        |
 
 
 ## Installation & Usage
 ### pip install
 Install the `manticoresearch` package with [pip](http://pypi.python.org)
 
 ```sh
@@ -94,29 +90,43 @@
     host = "http://127.0.0.1:9308"
 )
 
 
 
 # Enter a context with an instance of the API client
 with manticoresearch.ApiClient(configuration) as api_client:
-    # Create an instance of the API class
+    # Create an instance of the IndexApi API class
     api_instance = manticoresearch.IndexApi(api_client)
     body = "["'{\"insert\": {\"index\": \"test\", \"id\": 1, \"doc\": {\"title\": \"Title 1\"}}},\\n{\"insert\": {\"index\": \"test\", \"id\": 2, \"doc\": {\"title\": \"Title 2\"}}}'"]" # str | 
 
     try:
         # Bulk index operations
         api_response = api_instance.bulk(body)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling IndexApi->bulk: %s\n" % e)
     
+    
+    # Create an instance of the Search API class
+    api_instance = manticoresearch.SearchApi(api_client)
+
+    # Create SearchRequest
+    search_request = SearchRequest()
+    search_request.index='test'
+    search_request.fullltext_filter=QueryFilter('Title 1') 
+    
+    # The example passes only required values which don't have defaults set
+    try:
+        # Perform a search
+        api_response = api_instance.search(search_request)
+        pprint(api_response)
+    except manticoresearch.ApiException as e:
+        print("Exception when calling SearchApi->search: %s\n" % e)
 ```
 
 # Documentation
 
 
-Full documentation is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder.
+Full documentation on the API Endpoints and Models used is available in  [docs](https://github.com/manticoresoftware/manticoresearch-python/tree/master/docs) folder as listed below.
 
 Manticore Search server documentation: https://manual.manticoresearch.com.
 
-
-
```

### Comparing `manticoresearch-2.2.0/manticoresearch.egg-info/SOURCES.txt` & `manticoresearch-3.3.0/manticoresearch.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -15,24 +15,53 @@
 manticoresearch.egg-info/top_level.txt
 manticoresearch/api/__init__.py
 manticoresearch/api/index_api.py
 manticoresearch/api/search_api.py
 manticoresearch/api/utils_api.py
 manticoresearch/apis/__init__.py
 manticoresearch/model/__init__.py
+manticoresearch/model/aggregation.py
+manticoresearch/model/attr_filter.py
+manticoresearch/model/bool_filter.py
 manticoresearch/model/bulk_response.py
 manticoresearch/model/delete_document_request.py
 manticoresearch/model/delete_response.py
+manticoresearch/model/equals_filter.py
 manticoresearch/model/error_response.py
+manticoresearch/model/facet.py
+manticoresearch/model/filter_boolean.py
+manticoresearch/model/filter_number.py
+manticoresearch/model/filter_string.py
+manticoresearch/model/fulltext_filter.py
+manticoresearch/model/geo_distance_filter.py
+manticoresearch/model/geo_distance_filter_location_anchor.py
+manticoresearch/model/highlight.py
+manticoresearch/model/highlight_field.py
+manticoresearch/model/in_filter.py
 manticoresearch/model/insert_document_request.py
+manticoresearch/model/match_filter.py
+manticoresearch/model/match_op.py
+manticoresearch/model/match_op_filter.py
+manticoresearch/model/match_phrase_filter.py
+manticoresearch/model/not_filter_boolean.py
+manticoresearch/model/not_filter_number.py
+manticoresearch/model/not_filter_string.py
+manticoresearch/model/option.py
 manticoresearch/model/percolate_request.py
 manticoresearch/model/percolate_request_query.py
+manticoresearch/model/query_filter.py
+manticoresearch/model/range_filter.py
 manticoresearch/model/search_request.py
 manticoresearch/model/search_response.py
 manticoresearch/model/search_response_hits.py
+manticoresearch/model/sort_multiple.py
+manticoresearch/model/sort_mva.py
+manticoresearch/model/sort_order.py
+manticoresearch/model/source_by_rules.py
+manticoresearch/model/source_multiple.py
 manticoresearch/model/sql_response.py
 manticoresearch/model/success_response.py
 manticoresearch/model/update_document_request.py
 manticoresearch/model/update_response.py
 manticoresearch/models/__init__.py
 test/test.py
 test/test_index_api.py
```

### Comparing `manticoresearch-2.2.0/setup.py` & `manticoresearch-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 
 from setuptools import setup, find_packages
 from os import path
 
 NAME = "manticoresearch"
-VERSION = "2.2.0"
+VERSION = "3.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `manticoresearch-2.2.0/test/test.py` & `manticoresearch-3.3.0/test/test.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/test/test_index_api.py` & `manticoresearch-3.3.0/test/test_index_api.py`

 * *Files identical despite different names*

### Comparing `manticoresearch-2.2.0/test/test_search_api.py` & `manticoresearch-3.3.0/test/test_search_api.py`

 * *Files identical despite different names*

