# Comparing `tmp/lusid-notification-sdk-preview-0.1.716.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.717.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.716.tar", last modified: Wed May 31 15:01:57 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.717.tar", last modified: Thu Jun  1 09:48:44 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.716.tar` & `lusid-notification-sdk-preview-0.1.717.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8040 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4452 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      506 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27431 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10957 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9234 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11191 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    10603 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    12390 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)    14935 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9337 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    14867 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8012 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     9020 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15803 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:01:57.000000 lusid-notification-sdk-preview-0.1.716/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-05-31 15:01:23.000000 lusid-notification-sdk-preview-0.1.716/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27431 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9234 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6508 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    10603 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    14867 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    14424 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     9020 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15803 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 09:48:44.000000 lusid-notification-sdk-preview-0.1.717/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-01 09:48:16.000000 lusid-notification-sdk-preview-0.1.717/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.716/README.md` & `lusid-notification-sdk-preview-0.1.717/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.716
-- Package version: 0.1.716
+- API version: 0.1.717
+- Package version: 0.1.717
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.716"
+__version__ = "0.1.717"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.deliveries_api import DeliveriesApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/deliveries_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/manual_event_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.716'
+        header_params['X-LUSID-SDK-Version'] = '0.1.717'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.716/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.717/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.716\n"\
-               "SDK Package Version: 0.1.716".\
+               "Version of the API: 0.1.717\n"\
+               "SDK Package Version: 0.1.717".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/api_request_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/attempt.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/attempt_status.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/attempt_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/delivery.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/manual_event_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_delivery.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/sms_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/update_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.716
+    The version of the OpenAPI document: 0.1.717
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.717/lusid_notification/utilities/config_keys.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'api_url'": "{'env': 'FBN_NOTIFICATION_API_URL', 'config': 'notificationUrl'}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "access_token": {
         "config": "accessToken",
         "env": "FBN_ACCESS_TOKEN"
     },
     "api_url": {
-        "config": "notificationsUrl",
-        "env": "FBN_NOTIFICATIONS_API_URL"
+        "config": "notificationUrl",
+        "env": "FBN_NOTIFICATION_API_URL"
     },
     "app_name": {
         "config": "applicationName",
         "env": "FBN_APP_NAME"
     },
     "certificate_filename": {
         "config": "clientCertificate",
```

### Comparing `lusid-notification-sdk-preview-0.1.716/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.717/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.716/setup.py` & `lusid-notification-sdk-preview-0.1.717/setup.py`

 * *Files identical despite different names*

