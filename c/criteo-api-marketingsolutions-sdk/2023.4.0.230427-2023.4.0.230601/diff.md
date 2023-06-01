# Comparing `tmp/criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar.gz` & `tmp/criteo-api-marketingsolutions-sdk-2023.4.0.230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar", last modified: Thu Apr 27 13:29:39 2023, max compression
+gzip compressed data, was "criteo-api-marketingsolutions-sdk-2023.4.0.230601.tar", last modified: Thu Jun  1 16:05:47 2023, max compression
```

## Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427.tar` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601.tar`

### file list

```diff
@@ -1,141 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 13:29:39.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/audience_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66384 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.871372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11946 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/common_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problem_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problems_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 13:29:39.887372 criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-27 13:28:49.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/test_gateway_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.364531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-01 16:05:47.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-01 16:05:47.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:05:47.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 16:05:47.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 16:05:47.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.364531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.364531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/audience_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66384 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39252 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api_client_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.364531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16739 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/flow_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12763 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12330 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11788 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12836 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12512 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14392 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/common_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12127 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14244 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12471 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13416 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12153 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/problem_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/problems_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13219 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12063 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11692 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11737 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12474 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82575 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14252 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:05:47.380531 criteo-api-marketingsolutions-sdk-2023.4.0.230601/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-01 16:04:55.000000 criteo-api-marketingsolutions-sdk-2023.4.0.230601/test/test_gateway_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/README.md` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/README.md`

 * *Files 17% similar despite different names*

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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_04
 ```
 
 ### Manual Installation using [Setuptools](http://pypi.python.org/pypi/setuptools)
@@ -38,15 +38,19 @@
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_04
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criteo-api-marketingsolutions-sdk
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 criteo_api_marketingsolutions_v2023_04/api_client.py
 criteo_api_marketingsolutions_v2023_04/api_client_builder.py
 criteo_api_marketingsolutions_v2023_04/configuration.py
 criteo_api_marketingsolutions_v2023_04/criteo_api_client.py
 criteo_api_marketingsolutions_v2023_04/criteo_auth.py
 criteo_api_marketingsolutions_v2023_04/criteo_rest.py
 criteo_api_marketingsolutions_v2023_04/exceptions.py
+criteo_api_marketingsolutions_v2023_04/flow_constants.py
 criteo_api_marketingsolutions_v2023_04/model_utils.py
 criteo_api_marketingsolutions_v2023_04/rest.py
 criteo_api_marketingsolutions_v2023_04/api/__init__.py
 criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py
 criteo_api_marketingsolutions_v2023_04/api/analytics_api.py
 criteo_api_marketingsolutions_v2023_04/api/audience_api.py
 criteo_api_marketingsolutions_v2023_04/api/campaign_api.py
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,21 @@
     Criteo publicly exposed API  # noqa: E501
 
     The version of the OpenAPI document: 2023-04
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "2023.04.0.230427"
+__version__ = "2023.04.0.230601"
 
 # import ApiClient
 from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
 from criteo_api_marketingsolutions_v2023_04.criteo_api_client import CriteoApiClient
 from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
+from criteo_api_marketingsolutions_v2023_04 import flow_constants
 
 # import Configuration
 from criteo_api_marketingsolutions_v2023_04.configuration import Configuration
 
 # import exceptions
 from criteo_api_marketingsolutions_v2023_04.exceptions import OpenApiException
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/advertiser_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/analytics_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/audience_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/audience_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/campaign_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api/gateway_api.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/api_client.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/api_client.py`

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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/apis/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/configuration.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/configuration.py`

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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
 from criteo_api_marketingsolutions_v2023_04.criteo_rest import CriteoRESTClientObject
 
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_auth.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from datetime import datetime, timedelta
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiException
 from criteo_api_marketingsolutions_v2023_04.api_client import ApiClient
+from criteo_api_marketingsolutions_v2023_04 import flow_constants
 
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/criteo_rest.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/criteo_rest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from criteo_api_marketingsolutions_v2023_04.rest import RESTClientObject
 from criteo_api_marketingsolutions_v2023_04.criteo_auth import *
+from criteo_api_marketingsolutions_v2023_04 import flow_constants
 
 
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

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/exceptions.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/exceptions.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_delivery_limitations.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_frequency_capping.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_geo_location.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_search_filter.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/ad_set_targeting_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/application_summary_model_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_error.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_name_description.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/audience_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/basic_audience_definition.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_read_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_search_filters.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_search_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/common_problem.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/common_problem.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_amendment_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/contactlist_operation_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/criteo_api_error.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/criteo_api_warning.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/delete_audience_contact_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/delete_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/entity_of_portfolio_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/error_code_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/get_audiences_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/get_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/modify_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/new_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
-    globals()['NillableAdSetTargetingRuleValue'] = NillableAdSetTargetingRuleValue
 
-
-class NillableAdSetTargetingRule(ModelNormal):
+class NillableDateTime(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,32 +62,30 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'value': (NillableAdSetTargetingRuleValue,),  # noqa: E501
+            'value': (datetime, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -103,18 +97,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
-        """NillableAdSetTargetingRule - a model defined in OpenAPI
+        """NillableDateTime - a model defined in OpenAPI
 
         Args:
-            value (NillableAdSetTargetingRuleValue):
+            value (datetime, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -192,18 +186,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, value, *args, **kwargs):  # noqa: E501
-        """NillableAdSetTargetingRule - a model defined in OpenAPI
+        """NillableDateTime - a model defined in OpenAPI
 
         Args:
-            value (NillableAdSetTargetingRuleValue):
+            value (datetime, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule_value.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_date_time.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
-class NillableDateTime(ModelNormal):
+class NillableDecimal(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,15 +77,15 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'value': (datetime, none_type,),  # noqa: E501
+            'value': (float, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -97,18 +97,18 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
-        """NillableDateTime - a model defined in OpenAPI
+        """NillableDecimal - a model defined in OpenAPI
 
         Args:
-            value (datetime, none_type):
+            value (float, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -186,18 +186,18 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, value, *args, **kwargs):  # noqa: E501
-        """NillableDateTime - a model defined in OpenAPI
+        """NillableDecimal - a model defined in OpenAPI
 
         Args:
-            value (datetime, none_type):
+            value (float, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/nillable_decimal.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
+    globals()['NillableDecimal'] = NillableDecimal
 
-class NillableDecimal(ModelNormal):
+
+class PatchAdSetBidding(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,53 +66,52 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (float, none_type,),  # noqa: E501
+            'bid_amount': (NillableDecimal,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'value': 'value',  # noqa: E501
+        'bid_amount': 'bidAmount',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, value, *args, **kwargs):  # noqa: E501
-        """NillableDecimal - a model defined in OpenAPI
-
-        Args:
-            value (float, none_type):
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """PatchAdSetBidding - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,14 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            bid_amount (NillableDecimal): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -164,15 +168,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -185,19 +188,16 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, value, *args, **kwargs):  # noqa: E501
-        """NillableDecimal - a model defined in OpenAPI
-
-        Args:
-            value (float, none_type):
+    def __init__(self, *args, **kwargs):  # noqa: E501
+        """PatchAdSetBidding - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,14 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            bid_amount (NillableDecimal): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -251,15 +252,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.value = value
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.nillable_decimal import NillableDecimal
-    globals()['NillableDecimal'] = NillableDecimal
 
-
-class PatchAdSetBidding(ModelNormal):
+class PatchAdSetDisplayMultiplier(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -66,52 +62,50 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'bid_amount': (NillableDecimal,),  # noqa: E501
+            'display_multiplier': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'bid_amount': 'bidAmount',  # noqa: E501
+        'display_multiplier': 'displayMultiplier',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetBidding - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplier - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -136,15 +130,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            bid_amount (NillableDecimal): [optional]  # noqa: E501
+            display_multiplier (float): Any positive decimal value. To remove the impact of the Display Multiplier set it to 1. At most 4 decimals are supported. Additional decimals are rounded.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -189,15 +183,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetBidding - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplier - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +216,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            bid_amount (NillableDecimal): [optional]  # noqa: E501
+            display_multiplier (float): Any positive decimal value. To remove the impact of the Display Multiplier set it to 1. At most 4 decimals are supported. Additional decimals are rounded.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_list_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_category_bid_result_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
+    globals()['PatchAdSetDisplayMultiplierResource'] = PatchAdSetDisplayMultiplierResource
 
-class PatchAdSetDisplayMultiplier(ModelNormal):
+
+class PatchAdSetDisplayMultiplierListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -54,58 +58,62 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
+        ('data',): {
+        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'display_multiplier': (float,),  # noqa: E501
+            'data': ([PatchAdSetDisplayMultiplierResource],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'display_multiplier': 'displayMultiplier',  # noqa: E501
+        'data': 'data',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplier - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierListRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -130,15 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            display_multiplier (float): Any positive decimal value. To remove the impact of the Display Multiplier set it to 1. At most 4 decimals are supported. Additional decimals are rounded.. [optional]  # noqa: E501
+            data ([PatchAdSetDisplayMultiplierResource]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -183,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplier - a model defined in OpenAPI
+        """PatchAdSetDisplayMultiplierListRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -216,15 +224,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            display_multiplier (float): Any positive decimal value. To remove the impact of the Display Multiplier set it to 1. At most 4 decimals are supported. Additional decimals are rounded.. [optional]  # noqa: E501
+            data ([PatchAdSetDisplayMultiplierResource]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set_display_multiplier_resource import PatchAdSetDisplayMultiplierResource
-    globals()['PatchAdSetDisplayMultiplierResource'] = PatchAdSetDisplayMultiplierResource
+    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
+    globals()['PatchCampaignWriteResource'] = PatchCampaignWriteResource
 
 
-class PatchAdSetDisplayMultiplierListRequest(ModelNormal):
+class PatchCampaignListRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -85,15 +85,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'data': ([PatchAdSetDisplayMultiplierResource],),  # noqa: E501
+            'data': ([PatchCampaignWriteResource],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -105,15 +105,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierListRequest - a model defined in OpenAPI
+        """PatchCampaignListRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +138,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([PatchAdSetDisplayMultiplierResource]): [optional]  # noqa: E501
+            data ([PatchCampaignWriteResource]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +191,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchAdSetDisplayMultiplierListRequest - a model defined in OpenAPI
+        """PatchCampaignListRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,15 +224,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([PatchAdSetDisplayMultiplierResource]): [optional]  # noqa: E501
+            data ([PatchCampaignWriteResource]): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_display_multiplier_result_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_ad_set_scheduling.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_list_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_campaign_write_resource import PatchCampaignWriteResource
-    globals()['PatchCampaignWriteResource'] = PatchCampaignWriteResource
 
-
-class PatchCampaignListRequest(ModelNormal):
+class PatchResultCampaignReadResource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -58,62 +54,62 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('data',): {
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
-            'data': ([PatchCampaignWriteResource],),  # noqa: E501
+            'id': (str,),  # noqa: E501
+            'type': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'data': 'data',  # noqa: E501
+        'id': 'id',  # noqa: E501
+        'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
+        'id',  # noqa: E501
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchCampaignListRequest - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -138,15 +134,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([PatchCampaignWriteResource]): [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -191,15 +188,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchCampaignListRequest - a model defined in OpenAPI
+        """PatchResultCampaignReadResource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -224,15 +221,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            data ([PatchCampaignWriteResource]): [optional]  # noqa: E501
+            id (str): Id of the entity. [optional]  # noqa: E501
+            type (str): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_spend_limit.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_campaign_write_resource.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_list_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/patch_result_campaign_read_resource.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 
-class PatchResultCampaignReadResource(ModelNormal):
+class WriteModelAdSetId(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -92,24 +92,22 @@
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
-        'id',  # noqa: E501
-        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +133,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -188,15 +186,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """PatchResultCampaignReadResource - a model defined in OpenAPI
+        """WriteModelAdSetId - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -222,15 +220,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): [optional]  # noqa: E501
+            type (str): Canonical type name of the entity. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/placements_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/portfolio_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problem_details.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/problem_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/problems_details.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/problems_details.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_bidding.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_budget.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_ad_set_schedule.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_model_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/read_model_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience_request.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/replace_audience_response.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/request_ad_set_search.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/requests_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/requests_patch_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/response_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/response_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/responses_ad_set_id.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/responses_read_ad_set.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/statistics_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transactions_report_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_query_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_attributes.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_data_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_entity_message.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/transparency_report_file.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_ad_set_id.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,20 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
+def lazy_import():
+    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set import PatchAdSet
+    globals()['PatchAdSet'] = PatchAdSet
 
-class WriteModelAdSetId(ModelNormal):
+
+class WriteModelPatchAdSet(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -62,52 +66,56 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
+        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'type': (str,),  # noqa: E501
+            'attributes': (PatchAdSet,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'attributes': 'attributes',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WriteModelAdSetId - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -134,14 +142,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -186,15 +195,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WriteModelAdSetId - a model defined in OpenAPI
+        """WriteModelPatchAdSet - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -221,14 +230,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             id (str): Id of the entity. [optional]  # noqa: E501
             type (str): Canonical type name of the entity. [optional]  # noqa: E501
+            attributes (PatchAdSet): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model/write_model_patch_ad_set.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model/nillable_ad_set_targeting_rule.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from criteo_api_marketingsolutions_v2023_04.exceptions import ApiAttributeError
 
 
 def lazy_import():
-    from criteo_api_marketingsolutions_v2023_04.model.patch_ad_set import PatchAdSet
-    globals()['PatchAdSet'] = PatchAdSet
+    from criteo_api_marketingsolutions_v2023_04.model.nillable_ad_set_targeting_rule_value import NillableAdSetTargetingRuleValue
+    globals()['NillableAdSetTargetingRuleValue'] = NillableAdSetTargetingRuleValue
 
 
-class WriteModelPatchAdSet(ModelNormal):
+class NillableAdSetTargetingRule(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -83,39 +83,35 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'id': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
-            'attributes': (PatchAdSet,),  # noqa: E501
+            'value': (NillableAdSetTargetingRuleValue,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'id': 'id',  # noqa: E501
-        'type': 'type',  # noqa: E501
-        'attributes': 'attributes',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """WriteModelPatchAdSet - a model defined in OpenAPI
+        """NillableAdSetTargetingRule - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +136,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (PatchAdSet): [optional]  # noqa: E501
+            value (NillableAdSetTargetingRuleValue): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -195,15 +189,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """WriteModelPatchAdSet - a model defined in OpenAPI
+        """NillableAdSetTargetingRule - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -228,17 +222,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Id of the entity. [optional]  # noqa: E501
-            type (str): Canonical type name of the entity. [optional]  # noqa: E501
-            attributes (PatchAdSet): [optional]  # noqa: E501
+            value (NillableAdSetTargetingRuleValue): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/model_utils.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/model_utils.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/models/__init__.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/models/__init__.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/criteo_api_marketingsolutions_v2023_04/rest.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/criteo_api_marketingsolutions_v2023_04/rest.py`

 * *Files identical despite different names*

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/setup.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "criteo-api-marketingsolutions-sdk"
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
-pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427
+pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601
 ```
-(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230427`)
+(you may need to run `pip` with root permission: `sudo pip install criteo-api-marketingsolutions-sdk==2023.04.0.230601`)
 
 Then import the package:
 ```python
 import criteo_api_marketingsolutions_v2023_04
 ```
 
 Full documentation on [Github](https://github.com/criteo/criteo-api-python-sdk).
```

### Comparing `criteo-api-marketingsolutions-sdk-2023.4.0.230427/test/test_gateway_api.py` & `criteo-api-marketingsolutions-sdk-2023.4.0.230601/test/test_gateway_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import os
 
 from criteo_api_marketingsolutions_v2023_04.api.gateway_api import GatewayApi
 from criteo_api_marketingsolutions_v2023_04.api_client_builder import ApiClientBuilder
 from criteo_api_marketingsolutions_v2023_04.rest import ApiException
-from example_application import ExampleApplication
+from example_application_with_client_credentials import ExampleApplication
 
 class TestGatewayApi:
   @pytest.fixture(autouse=True)
   def before_each(self):
     self.client_id = os.environ.get("TEST_CLIENT_ID")
     self.client_secret = os.environ.get("TEST_CLIENT_SECRET")
     self.application_id = int(os.environ.get("TEST_APPLICATION_ID"))
```

