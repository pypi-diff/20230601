# Comparing `tmp/moiz-gillani-whatsapp-cloud-api-sdk-1.0.1.tar.gz` & `tmp/moiz-gillani-whatsapp-cloud-api-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moiz-gillani-whatsapp-cloud-api-sdk-1.0.1.tar", last modified: Thu Jun  1 13:00:25 2023, max compression
+gzip compressed data, was "moiz-gillani-whatsapp-cloud-api-sdk-1.0.2.tar", last modified: Thu Jun  1 13:16:47 2023, max compression
```

## Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1.tar` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.832341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5358 2023-06-01 13:00:25.832341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4912 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.754341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5358 2023-06-01 13:00:25.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3852 2023-06-01 13:00:25.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:00:25.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 13:00:25.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 13:00:25.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      822 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 13:00:25.833341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.758340 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/api_helper.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.766341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1974 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/base_controller.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/business_profiles_controller.py
--rw-r--r--   0 root         (0) root         (0)     7668 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/media_controller.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/messages_controller.py
--rw-r--r--   0 root         (0) root         (0)     7086 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/phone_numbers_controller.py
--rw-r--r--   0 root         (0) root         (0)     5093 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/registration_controller.py
--rw-r--r--   0 root         (0) root         (0)     3370 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/two_step_verification_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.768341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/exceptions/
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/exceptions/api_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.774341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.776341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/auth/
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/auth/o_auth_2.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_call_back.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_request.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.829341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/
--rw-r--r--   0 root         (0) root         (0)     1375 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/action.py
--rw-r--r--   0 root         (0) root         (0)     3572 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/address.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/audio.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/body.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/business_profile.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/button.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/button_parameter.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/button_parameter_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2920 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/component.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/component_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/contact.py
--rw-r--r--   0 root         (0) root         (0)      413 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/content_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/currency.py
--rw-r--r--   0 root         (0) root         (0)     4169 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/date_time_object.py
--rw-r--r--   0 root         (0) root         (0)     2770 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/document.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/email_object.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/footer.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/get_business_profile_id_response.py
--rw-r--r--   0 root         (0) root         (0)     2676 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/get_phone_number_by_id_response.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/header.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/header_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/image.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/interactive.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/interactive_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     1883 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/language.py
--rw-r--r--   0 root         (0) root         (0)     2495 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/location.py
--rw-r--r--   0 root         (0) root         (0)     7908 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/message.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/message_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/name.py
--rw-r--r--   0 root         (0) root         (0)     2292 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/org.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/parameter_type_enum.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/personal_information_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     2274 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/phone_object.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/phone_type_enum.py
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/quality_rating_enum.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/register_phone_request.py
--rw-r--r--   0 root         (0) root         (0)      469 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/request_verification_code_method_enum.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/request_verification_code_request.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/response_contact.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/response_message.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/retrieve_media_url_response.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/row.py
--rw-r--r--   0 root         (0) root         (0)     2406 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/section.py
--rw-r--r--   0 root         (0) root         (0)     2451 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/send_message_response.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/set_two_step_verification_code_request.py
--rw-r--r--   0 root         (0) root         (0)     2013 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/sticker.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/sub_type_enum.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/success_response.py
--rw-r--r--   0 root         (0) root         (0)     2588 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/template.py
--rw-r--r--   0 root         (0) root         (0)     3023 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/text.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/update_business_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1379 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/upload_media.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/upload_media_request.py
--rw-r--r--   0 root         (0) root         (0)     1888 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/url_object.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/verify_code_request.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/vertical_enum.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/video.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:00:25.831341 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/utilities/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/utilities/file_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-06-01 12:59:55.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/whatsappcloudapi_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.325762 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-06-01 13:16:47.325762 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.245761 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5358 2023-06-01 13:16:47.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-06-01 13:16:47.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:16:47.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 13:16:47.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 13:16:47.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      822 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-01 13:16:47.328762 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.249760 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/api_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.260761 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1974 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/base_controller.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/business_profiles_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7668 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/media_controller.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/messages_controller.py
+-rw-r--r--   0 root         (0) root         (0)     7086 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/phone_numbers_controller.py
+-rw-r--r--   0 root         (0) root         (0)     5093 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/registration_controller.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/two_step_verification_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.262761 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/exceptions/
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/exceptions/api_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.268761 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.277761 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/auth/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/auth/o_auth_2.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_call_back.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_request.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.324762 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/audio.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/body.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/business_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/button.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/button_parameter.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/button_parameter_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2920 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/component.py
+-rw-r--r--   0 root         (0) root         (0)      514 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/component_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/contact.py
+-rw-r--r--   0 root         (0) root         (0)      413 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/content_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/currency.py
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/date_time_object.py
+-rw-r--r--   0 root         (0) root         (0)     2770 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/document.py
+-rw-r--r--   0 root         (0) root         (0)     1918 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/email_object.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/footer.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/get_business_profile_id_response.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/get_phone_number_by_id_response.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/header.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/header_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/image.py
+-rw-r--r--   0 root         (0) root         (0)     3159 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/interactive.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/interactive_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1883 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/language.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/message_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/name.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/org.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/parameter_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/personal_information_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/phone_object.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/phone_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/quality_rating_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/register_phone_request.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/request_verification_code_method_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/request_verification_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/response_contact.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/response_message.py
+-rw-r--r--   0 root         (0) root         (0)     2840 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/retrieve_media_url_response.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/row.py
+-rw-r--r--   0 root         (0) root         (0)     2406 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/section.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/send_message_response.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/set_two_step_verification_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/sticker.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/sub_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/success_response.py
+-rw-r--r--   0 root         (0) root         (0)     2588 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/template.py
+-rw-r--r--   0 root         (0) root         (0)     3023 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/text.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/update_business_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/upload_media.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/upload_media_request.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/url_object.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/verify_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/vertical_enum.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/video.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:16:47.325762 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/utilities/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/utilities/file_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-01 13:16:19.000000 moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/whatsappcloudapi_client.py
```

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/LICENSE` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/PKG-INFO` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moiz-gillani-whatsapp-cloud-api-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use cloud-hosted version of the WhatsApp Business API to send and receive messages
 Author-email: moiz gillani <moiz.gillani@apimatic.io>
 Project-URL: Documentation, https://dev.apimatic.io/api-docs-preview/dashboard/64789018957008f48600193d/v/1_0#/http/step-by-step-tutorial
 Keywords: whatsapp,messages,api
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -32,23 +32,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.1
+pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.1
+https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.2
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `version` | `string` | *Default*: `'v13.0'` |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
@@ -75,20 +75,20 @@
 
 ## Authorization
 
 This API uses `OAuth 2 Bearer token`.
 
 ## List of APIs
 
-* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/business-profiles.md)
-* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/phone-numbers.md)
-* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/two-step-verification.md)
-* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/messages.md)
-* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/registration.md)
-* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/media.md)
+* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/business-profiles.md)
+* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/phone-numbers.md)
+* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/two-step-verification.md)
+* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/messages.md)
+* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/registration.md)
+* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/media.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-request.md)
```

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/README.md` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.1
+pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.1
+https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.2
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `version` | `string` | *Default*: `'v13.0'` |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
@@ -63,20 +63,20 @@
 
 ## Authorization
 
 This API uses `OAuth 2 Bearer token`.
 
 ## List of APIs
 
-* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/business-profiles.md)
-* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/phone-numbers.md)
-* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/two-step-verification.md)
-* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/messages.md)
-* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/registration.md)
-* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/media.md)
+* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/business-profiles.md)
+* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/phone-numbers.md)
+* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/two-step-verification.md)
+* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/messages.md)
+* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/registration.md)
+* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/media.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-request.md)
```

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/PKG-INFO` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moiz-gillani-whatsapp-cloud-api-sdk
-Version: 1.0.1
+Version: 1.0.2
 Summary: Use cloud-hosted version of the WhatsApp Business API to send and receive messages
 Author-email: moiz gillani <moiz.gillani@apimatic.io>
 Project-URL: Documentation, https://dev.apimatic.io/api-docs-preview/dashboard/64789018957008f48600193d/v/1_0#/http/step-by-step-tutorial
 Keywords: whatsapp,messages,api
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testutils
@@ -32,23 +32,23 @@
 
 ## Install the Package
 
 The package is compatible with Python versions `3 >=3.7, <= 3.11`.
 Install the package from PyPi using the following pip command:
 
 ```python
-pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.1
+pip install moiz-gillani-whatsapp-cloud-api-sdk==1.0.2
 ```
 
 You can also view the package at:
-https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.1
+https://pypi.python.org/pypi/moiz-gillani-whatsapp-cloud-api-sdk/1.0.2
 
 ## Initialize the API Client
 
-**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/client.md)
+**_Note:_** Documentation for the client can be found [here.](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/client.md)
 
 The following parameters are configurable for the API Client:
 
 | Parameter | Type | Description |
 |  --- | --- | --- |
 | `version` | `string` | *Default*: `'v13.0'` |
 | `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
@@ -75,20 +75,20 @@
 
 ## Authorization
 
 This API uses `OAuth 2 Bearer token`.
 
 ## List of APIs
 
-* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/business-profiles.md)
-* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/phone-numbers.md)
-* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/two-step-verification.md)
-* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/messages.md)
-* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/registration.md)
-* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/controllers/media.md)
+* [Business Profiles](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/business-profiles.md)
+* [Phone Numbers](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/phone-numbers.md)
+* [Two-Step Verification](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/two-step-verification.md)
+* [Messages](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/messages.md)
+* [Registration](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/registration.md)
+* [Media](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/controllers/media.md)
 
 ## Classes Documentation
 
-* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/utility-classes.md)
-* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-response.md)
-* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.1/doc/http-request.md)
+* [Utility Classes](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/utility-classes.md)
+* [HttpResponse](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-response.md)
+* [HttpRequest](https://www.github.com/moizgillani/whatsapp-cloud-api-python-sdk/tree/1.0.2/doc/http-request.md)
```

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/SOURCES.txt` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/moiz_gillani_whatsapp_cloud_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/pyproject.toml` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0"]
 [project]
 name = "moiz-gillani-whatsapp-cloud-api-sdk"
 description = "Use cloud-hosted version of the WhatsApp Business API to send and receive messages"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["whatsapp", "messages", "api"]
 authors = [{name = "moiz gillani", email = "moiz.gillani@apimatic.io"}]
 urls = {Documentation = "https://dev.apimatic.io/api-docs-preview/dashboard/64789018957008f48600193d/v/1_0#/http/step-by-step-tutorial"}
 dependencies = ["apimatic-core~=0.2.0", "apimatic-core-interfaces~=0.1.0", "apimatic-requests-client-adapter~=0.1.0", "python-dateutil~=2.8.1", "enum34~=1.1, >=1.1.10"]
 classifiers = []
```

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/api_helper.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/api_helper.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/configuration.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/configuration.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/base_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/business_profiles_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/business_profiles_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/media_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/media_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/messages_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/messages_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/phone_numbers_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/phone_numbers_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/registration_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/registration_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/controllers/two_step_verification_controller.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/controllers/two_step_verification_controller.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/exceptions/api_exception.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/exceptions/api_exception.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/auth/o_auth_2.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/auth/o_auth_2.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/http/http_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/http/http_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/__init__.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/action.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/action.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/address.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/address.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/audio.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/audio.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/body.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/body.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/business_profile.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/business_profile.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/button.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/button.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/button_parameter.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/button_parameter.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/component.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/component.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/component_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/component_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/contact.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/contact.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/currency.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/currency.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/date_time_object.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/date_time_object.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/document.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/document.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/email_object.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/email_object.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/footer.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/footer.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/get_business_profile_id_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/get_business_profile_id_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/get_phone_number_by_id_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/get_phone_number_by_id_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/header.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/header.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/header_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/header_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/image.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/image.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/interactive.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/interactive.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/language.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/language.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/location.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/location.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/message.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/message.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/message_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/message_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/name.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/name.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/org.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/org.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/parameter.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/parameter.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/parameter_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/parameter_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/phone_object.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/phone_object.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/phone_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/phone_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/quality_rating_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/quality_rating_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/register_phone_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/register_phone_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/request_verification_code_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/request_verification_code_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/response_contact.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/response_contact.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/response_message.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/response_message.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/retrieve_media_url_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/retrieve_media_url_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/row.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/row.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/section.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/section.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/send_message_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/send_message_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/set_two_step_verification_code_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/set_two_step_verification_code_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/sticker.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/sticker.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/sub_type_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/sub_type_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/success_response.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/success_response.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/template.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/template.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/text.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/text.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/update_business_profile_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/update_business_profile_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/upload_media.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/upload_media.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/upload_media_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/upload_media_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/url_object.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/url_object.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/verify_code_request.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/verify_code_request.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/vertical_enum.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/vertical_enum.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/models/video.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/models/video.py`

 * *Files identical despite different names*

### Comparing `moiz-gillani-whatsapp-cloud-api-sdk-1.0.1/whatsappcloudapi/whatsappcloudapi_client.py` & `moiz-gillani-whatsapp-cloud-api-sdk-1.0.2/whatsappcloudapi/whatsappcloudapi_client.py`

 * *Files identical despite different names*

