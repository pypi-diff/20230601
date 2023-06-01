# Comparing `tmp/criteo-api-retailmedia-sdk-2023.4.0.230427.tar.gz` & `tmp/criteo-api-retailmedia-sdk-2023.4.0.230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-retailmedia-sdk-2023.4.0.230427.tar", last modified: Thu Apr 27 13:30:51 2023, max compression
+gzip compressed data, was "criteo-api-retailmedia-sdk-2023.4.0.230601.tar", last modified: Thu Jun  1 16:07:00 2023, max compression
```

## Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427.tar` & `criteo-api-retailmedia-sdk-2023.4.0.230601.tar`

### file list

```diff
@@ -1,218 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.916910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:30:50.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   369292 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.920910 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.992911 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/color_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/customer_list_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/map_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_type_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
--rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
--rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/section.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
--rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.992911 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:30:50.996911 criteo-api-retailmedia-sdk-2023.4.0.230427/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-27 13:28:49.000000 criteo-api-retailmedia-sdk-2023.4.0.230427/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.004911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-01 16:06:59.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-06-01 16:07:00.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:06:59.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 16:06:59.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 16:06:59.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.008911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.008911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25929 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   369292 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39223 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.008911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12754 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16280 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18461 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/color_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12766 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12563 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/customer_list_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11667 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16679 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15104 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16312 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/files_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12110 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12985 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11951 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12927 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/map_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/page_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/page_type_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12472 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11953 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12313 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12191 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12132 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12215 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12393 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12448 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12358 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12112 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12082 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12266 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13516 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12257 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11809 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16101 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11592 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/text_variable_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82568 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:07:00.032911 criteo-api-retailmedia-sdk-2023.4.0.230601/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-01 16:04:55.000000 criteo-api-retailmedia-sdk-2023.4.0.230601/test/test_gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.4.0.230601/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.4.0.230427
+Version: 2023.4.0.230601
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/README.md` & `criteo-api-retailmedia-sdk-2023.4.0.230601/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 API Client Libraries can facilitate your use of the Criteo API allowing you to build unique and customized solutions to serve your businesses and clients.
 These libraries can reduce the amount of code you need to write in order to start accessing Criteo programmatically. They also can help expedite troubleshooting, should you encounter any issues.
 
 More information: [https://developers.criteo.com/](https://developers.criteo.com/)
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- Package version: 2023.04.0.230427
+- Package version: 2023.04.0.230601
 
 ## Requirements
 
 Python 2.7 and 3.5+
 
 ## Installation & Usage
 ### pip install
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
@@ -38,15 +38,19 @@
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_04
 ```
 
 ## Example
-Please see [test/example_application.py](test/example_application.py) for an example.
+There are multiple examples for the different OAuth flows that the SDK supports.
+- See [test/example_application_with_client_credentials.py](test/example_application_with_client_credentials.py) for an example with Client Credentials.
+- See [test/example_application_with_auth_code.py](test/example_application_with_auth_code.py) for an example with Authorization Code.
+Once you follow the authorization code flow, you will have a refresh token that has to be used to regenerate access token for future usage. 
+    - See [test/example_application_with_refresh_token.py](test/example_application_with_refresh_token.py) for an example with Refresh Token .
 
 ## Documentation for API Endpoints
 
 The developers documentation is available at: *https://developers.criteo.com*.
 
 All URIs are relative to *https://api.criteo.com*.
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/PKG-INFO` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-retailmedia-sdk
-Version: 2023.4.0.230427
+Version: 2023.4.0.230601
 Summary: Criteo API SDK
 Home-page: https://github.com/criteo/criteo-api-python-sdk
 Author: Criteo
 Author-email: 
 Keywords: Criteo,OpenAPI-Generator,Criteo API SDK
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,17 +20,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 criteo_api_retailmedia_v2023_04/api_client.py
 criteo_api_retailmedia_v2023_04/api_client_builder.py
 criteo_api_retailmedia_v2023_04/configuration.py
 criteo_api_retailmedia_v2023_04/criteo_api_client.py
 criteo_api_retailmedia_v2023_04/criteo_auth.py
 criteo_api_retailmedia_v2023_04/criteo_rest.py
 criteo_api_retailmedia_v2023_04/exceptions.py
+criteo_api_retailmedia_v2023_04/flow_constants.py
 criteo_api_retailmedia_v2023_04/model_utils.py
 criteo_api_retailmedia_v2023_04/rest.py
 criteo_api_retailmedia_v2023_04/api/__init__.py
 criteo_api_retailmedia_v2023_04/api/analytics_api.py
 criteo_api_retailmedia_v2023_04/api/audience_api.py
 criteo_api_retailmedia_v2023_04/api/campaign_api.py
 criteo_api_retailmedia_v2023_04/api/gateway_api.py
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     Criteo publicly exposed API  # noqa: E501
 
     The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.04.0.230427"
+__version__ = "2023.04.0.230601"
 
 # import ApiClient
 from criteo_api_retailmedia_v2023_04.api_client import ApiClient
 from criteo_api_retailmedia_v2023_04.criteo_api_client import CriteoApiClient
 from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
+from criteo_api_retailmedia_v2023_04 import flow_constants
 
 # import Configuration
 from criteo_api_retailmedia_v2023_04.configuration import Configuration
 
 # import exceptions
 from criteo_api_retailmedia_v2023_04.exceptions import OpenApiException
 from criteo_api_retailmedia_v2023_04.exceptions import ApiAttributeError
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/analytics_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/audience_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/campaign_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api/gateway_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/api_client.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2023.04.0.230427/python'
+        self.user_agent = 'OpenAPI-Generator/2023.04.0.230601/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/apis/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/configuration.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2023-04\n"\
-               "SDK Package Version: 2023.04.0.230427".\
+               "SDK Package Version: 2023.04.0.230601".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_api_client.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_api_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from criteo_api_retailmedia_v2023_04.api_client import ApiClient
 from criteo_api_retailmedia_v2023_04.criteo_rest import CriteoRESTClientObject
 
 class CriteoApiClient(ApiClient):
     def __init__(self, configuration=None, header_name=None, header_value=None,
              cookie=None, pool_threads=1, additional_parameters= {}):
         super().__init__(configuration=configuration,header_name=header_name, header_value=header_value, cookie=cookie, pool_threads=pool_threads)
-        self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
+        self.rest_client = CriteoRESTClientObject(self.configuration, additional_parameters)
+
+    def get_refresh_token(self):
+        return self.rest_client.get_refresh_token()
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_auth.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from datetime import datetime, timedelta
 from criteo_api_retailmedia_v2023_04.exceptions import ApiException
 from criteo_api_retailmedia_v2023_04.api_client import ApiClient
+from criteo_api_retailmedia_v2023_04 import flow_constants
 
 class Token(object):
 
     def __init__(self, token_string , expiration_date = None):
         self.expiration_date = expiration_date 
         self.token_string = token_string
 
@@ -25,18 +26,21 @@
 class RetryingOAuth(object):
 
     def __init__(self, grant_type, client_id, client_secret):
         self.grant_type = grant_type
         self.client_id = client_id
         self.client_secret = client_secret
         self.token = None
+        self.refreshToken = None
 
     def get_token(self, client : ApiClient, headers) -> str:    
         if self.token and not self.token.has_expired():
             self.token = None
+            if self.grant_type == flow_constants.AUTHORIZATION_CODE_FLOW:
+                self.grant_type = flow_constants.REFRESH_TOKEN_FLOW
 
         if self.token is None:
             self.refresh_token(client, headers)
 
         return self.token   
 
     def refresh_token(self, client : ApiClient, headers, parameters_dict= {}):
@@ -46,30 +50,37 @@
                        'User-Agent': headers['User-Agent']}
         params = dict(parameters_dict, **{
             'client_id':  self.client_id,
             'client_secret': self.client_secret,
             'grant_type' : self.grant_type 
             })
         try:
+            if self.grant_type == flow_constants.REFRESH_TOKEN_FLOW:
+                params['refresh_token'] = self.refreshToken
+
             response = client.request('POST', oauth_url,
                                     headers=new_headers,
                                     query_params=[],
                                     post_params=list(params.items()),
                                     _preload_content=True,
                                     _request_timeout=None,
                                     body=None,
                                     no_auth=True)
             data = json.loads(response.data)
             self.token = Token('Bearer '+ (data['access_token'] or ''),
                RetryingOAuth.compute_expiration_date(data['expires_in']))
-
+            self.refreshToken = data['refresh_token']
+            
             return self.token
         except ApiException as e:
             raise self._enrich_exception_message(e, oauth_url)
 
+    def get_refresh_token(self):
+        return self.refreshToken
+
     def _enrich_exception_message(self, e, url):
         try:
             data = json.loads(e.body or {})
         except ValueError:
             data = {}
         data['token_error'] = "Cannot refresh token by calling '" + url + "'"
         e.body = json.dumps(data).encode()
@@ -78,22 +89,33 @@
     @staticmethod
     def compute_expiration_date(expires_in):
         return datetime.utcnow() + timedelta(seconds=int(expires_in) + 15)
 
 class RetryingClientCredentials(RetryingOAuth):
     
     def __init__(self, client_id, client_secret):
-        super().__init__('client_credentials', client_id, client_secret)
+        super().__init__(flow_constants.CLIENT_CREDENTIALS_FLOW, client_id, client_secret)
 
 class RetryingAuthorizationCode(RetryingOAuth):
-   
     def __init__(self, client_id, client_secret, code, redirect_uri):
-        super().__init__('authorization_code', client_id, client_secret)
+        super().__init__(flow_constants.AUTHORIZATION_CODE_FLOW, client_id, client_secret)
         self.authorization_code = code
         self.redirect_uri = redirect_uri
 
     def refresh_token(self, client : ApiClient, headers, parameters_dict= {}):  
         params = dict(parameters_dict, **{
-            'authorization_code' : self.authorization_code,
+            'code' : self.authorization_code,
             'redirect_uri' : self.redirect_uri
         })
         return super().refresh_token(client, headers, params)
+    
+class RetryingRefreshToken(RetryingOAuth):
+
+    def __init__(self, client_id, client_secret, refresh_token):
+        super().__init__(flow_constants.REFRESH_TOKEN_FLOW, client_id, client_secret)
+        self.refreshToken = refresh_token
+
+    def refresh_token(self, client: ApiClient, headers, parameters_dict = {}):
+        params = dict(parameters_dict, **{
+            'refresh_token' : self.refreshToken
+        })
+        return super().refresh_token(client, headers,params)
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/criteo_rest.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/criteo_rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from criteo_api_retailmedia_v2023_04.rest import RESTClientObject
 from criteo_api_retailmedia_v2023_04.criteo_auth import *
+from criteo_api_retailmedia_v2023_04 import flow_constants
 
 
 class CriteoRESTClientObject(RESTClientObject):
 
     def __init__(self, configuration, additional_parameters = {}, pools_size=4, maxsize=None):
         super().__init__(configuration, pools_size, maxsize)
 
         self.host = configuration.host
         client_id = configuration.username
         client_secret = configuration.password
 
         grant_type = additional_parameters.get('flow', 'client_credentials')
-        if grant_type == 'authorization_code' :
+        if grant_type == flow_constants.AUTHORIZATION_CODE_FLOW :
             self.authorization = RetryingAuthorizationCode(
                 client_id,
                 client_secret, 
-                additional_parameters.get('autorization_code',''),
+                additional_parameters.get('authorization_code',''),
                 additional_parameters.get('redirect_uri','')
             )
+        elif grant_type == flow_constants.REFRESH_TOKEN_FLOW :
+             self.authorization = RetryingRefreshToken(
+                  client_id,
+                  client_secret,
+                  additional_parameters.get('refresh_token', '')
+             )
         else:
             self.authorization = RetryingClientCredentials(
                 client_id,
                 client_secret
             )
 
     def request(self, method, url, query_params=None, headers=None,
@@ -60,7 +67,9 @@
             headers['Authorization'] = token.token_string
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/json'
 
         return super().request(method, url, query_params, headers, body, post_params, _preload_content, _request_timeout)
 
+    def get_refresh_token(self):
+         return self.authorization.get_refresh_token()
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/exceptions.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/add_to_basket_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/asset_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/asset_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_create_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/auction_line_item_update_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/audience_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/bad_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/bad_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/balance_campaign202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/category202204_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_option.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_option.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/choice_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/color_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/color_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_error.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_line_item_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_line_item_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_problem.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_status_code_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/common_warning.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/common_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_body.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_data.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_retail_media_audience_v2_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/create_user_behavior_segment_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202110_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative202210_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative202210_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative_create_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/creative_update_model202207.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/customer_list_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/customer_list_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/editable_campaign_attributes_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/envelope_report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/envelope_report_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/error.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_auction_line_item_update_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_balance202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_balance202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_common_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_capping202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_page202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_line_item_page_category202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_retailer_pages202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_store_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/external_store_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/files_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/files_variables_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/get_page_of_audiences_by_account_id_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/hyperlink_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/input_resource_of_auction_line_item_create_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/input_resource_of_preferred_line_item_create_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_external_id_of_editable_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_account_and_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_brand_and_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_campaign_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_catalog_status_and_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_line_item_bid_multipliers_and_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_with_id_of_int64_and_retailer_and_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_campaign_attributes_v202301_and_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_body_without_id_of_catalog_request_and_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_account.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_brand.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_page_response_of_retailer.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_request_of_catalog_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_catalog_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/json_api_single_response_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/keyword_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/keyword_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/line_item_bid_multipliers_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/map_string.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/map_string.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_metadata.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/page_metadata.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/page_type_environment.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/page_type_environment.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/post_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item_create_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/preferred_line_item_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/problem_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/promoted_product202110_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/promoted_product202110_paged_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/put_campaign_v202301.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_request_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_status.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/report_status_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_auction_line_item_update_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_balance202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_balance_campaign202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_category202204.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_common_line_item.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_creative202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_creative202210.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_line_item_bid_multipliers.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_preferred_line_item_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_promoted_product202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/resource_of_template.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/resource_of_template.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_audience_v2_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keyword_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_add_remove_keywords_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_input_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keyword_data_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_keywords_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_proposal_status_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_resource_outcome.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bid_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/retail_media_externalv1_set_bids_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/section.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/section.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_ids_update_model202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_target202110_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/store_target202110_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_list_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_response.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_variable.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/template_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/template_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/text_variable_specification.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/text_variable_value.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/text_variable_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/user_behavior_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/user_behavior_details_v2.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_add_to_basket_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_audience_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_keyword_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_ids_update_model202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model/value_type_resource_of_store_target202110.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/model_utils.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/models/__init__.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/models/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/criteo_api_retailmedia_v2023_04/rest.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/criteo_api_retailmedia_v2023_04/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/setup.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-retailmedia-sdk"
-VERSION = "2023.04.0.230427"
+VERSION = "2023.04.0.230601"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -20,17 +20,17 @@
 IMPORTANT: This Python package links to Criteo production environment. Any test applied here will thus impact real data.
 
 ## Installation & Usage
 ### pip install
 
 
 ```sh
-pip install criteo-api-retailmedia-sdk==2023.04.0.230427
+pip install criteo-api-retailmedia-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-retailmedia-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_retailmedia_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-retailmedia-sdk-2023.4.0.230427/test/test_gateway_api.py` & `criteo-api-retailmedia-sdk-2023.4.0.230601/test/test_gateway_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import os
 
 from criteo_api_retailmedia_v2023_04.api.gateway_api import GatewayApi
 from criteo_api_retailmedia_v2023_04.api_client_builder import ApiClientBuilder
 from criteo_api_retailmedia_v2023_04.rest import ApiException
-from example_application import ExampleApplication
+from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
     self.application_id = int(os.environ.get("TEST_APPLICATION_ID"))
```

