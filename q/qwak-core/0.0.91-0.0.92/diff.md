# Comparing `tmp/qwak_core-0.0.91.tar.gz` & `tmp/qwak_core-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.91.tar", max compression
+gzip compressed data, was "qwak_core-0.0.92.tar", max compression
```

## Comparing `qwak_core-0.0.91.tar` & `qwak_core-0.0.92.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-05-31 10:21:45.584519 qwak_core-0.0.91/README.md
--rw-r--r--   0        0        0        0 2023-05-31 10:23:39.145215 qwak_core-0.0.91/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-31 10:23:39.177215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-31 10:23:15.745073 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.177215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-31 10:23:39.173215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-31 10:23:15.309071 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.173215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-31 10:23:39.173215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-31 10:23:15.549072 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.173215 qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-31 10:23:39.165215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-31 10:23:14.701067 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-31 10:23:39.165215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-31 10:23:39.165215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-31 10:23:14.893068 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.165215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-05-31 10:23:39.169215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-05-31 10:23:15.093069 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.169215 qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-31 10:23:39.149215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-31 10:23:14.509066 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-31 10:23:39.149215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-05-31 10:23:39.149215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-05-31 10:23:15.953075 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.153215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-31 10:23:39.157215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-31 10:23:16.353077 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.157215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-31 10:23:39.157215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-31 10:23:16.557078 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-31 10:23:39.161215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-31 10:23:39.153215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-31 10:23:16.149076 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.153215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-31 10:23:39.161215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-31 10:23:16.753080 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.161215 qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-31 10:23:39.213216 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-31 10:23:19.513096 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.217216 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-31 10:23:39.217216 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-31 10:23:19.705097 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-31 10:23:39.217216 qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-31 10:23:39.301216 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-31 10:23:25.673133 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.301216 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-31 10:23:39.301216 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-31 10:23:25.877135 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-31 10:23:39.305216 qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-31 10:23:39.309216 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-31 10:23:26.853141 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-31 10:23:39.309216 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-31 10:23:39.305216 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-31 10:23:26.665140 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.305216 qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-31 10:23:39.309216 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-31 10:23:27.049142 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.313216 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-31 10:23:39.313216 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-31 10:23:27.241143 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-31 10:23:39.313216 qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-31 10:23:39.417217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-31 10:23:36.405199 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.417217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-31 10:23:39.409217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-31 10:23:35.965196 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.413217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-31 10:23:39.413217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-31 10:23:36.189197 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.413217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-31 10:23:39.405217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-31 10:23:35.521193 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-31 10:23:39.405217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-31 10:23:39.409217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-31 10:23:35.733194 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.409217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-31 10:23:39.421217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-31 10:23:37.081203 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.425217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-31 10:23:39.421217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-31 10:23:36.857201 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.421217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-31 10:23:39.417217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-31 10:23:36.617200 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.417217 qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-31 10:23:39.405217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-31 10:23:35.273192 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.405217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-31 10:23:39.397217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-31 10:23:34.821189 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.397217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-31 10:23:39.401217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-31 10:23:35.053190 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-31 10:23:39.401217 qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-31 10:23:39.341216 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-31 10:23:29.269155 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-31 10:23:39.341216 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-31 10:23:39.337216 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-31 10:23:29.061154 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.341216 qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-05-31 10:23:39.329216 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-05-31 10:23:28.661152 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.329216 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-31 10:23:39.333216 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-31 10:23:28.853153 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.333216 qwak_core-0.0.91/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-31 10:23:39.333216 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-31 10:23:29.473157 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-31 10:23:39.333216 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-05-31 10:23:39.337216 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-05-31 10:23:29.909159 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-31 10:23:39.337216 qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-31 10:23:39.349217 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-31 10:23:30.325162 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.349217 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-31 10:23:39.349217 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-31 10:23:30.537163 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-31 10:23:39.353217 qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-31 10:23:39.321216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-31 10:23:28.057148 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.325216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-31 10:23:39.325216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-31 10:23:28.261149 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-31 10:23:39.325216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-31 10:23:39.317216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-31 10:23:27.649145 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.317216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-31 10:23:39.317216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-31 10:23:27.453144 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.317216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-31 10:23:39.321216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-31 10:23:27.861147 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-31 10:23:39.321216 qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-31 10:23:39.201216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-31 10:23:18.549090 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.201216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-31 10:23:39.205216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-31 10:23:18.745092 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.205216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-31 10:23:39.205216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-31 10:23:18.941093 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-31 10:23:39.209216 qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-31 10:23:39.277216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-31 10:23:24.513126 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.281216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-31 10:23:39.277216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-31 10:23:24.317125 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-31 10:23:39.277216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-31 10:23:39.245216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-31 10:23:22.125112 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.245216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-31 10:23:39.241216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-31 10:23:21.925111 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.245216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-31 10:23:39.237216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-31 10:23:21.289107 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.237216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-31 10:23:39.241216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-31 10:23:21.733110 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-31 10:23:39.241216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-31 10:23:39.249216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-31 10:23:22.329113 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.249216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-31 10:23:39.249216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-31 10:23:22.529115 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-31 10:23:39.253216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-05-31 10:23:39.237216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-05-31 10:23:21.501108 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.237216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-31 10:23:39.253216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-31 10:23:22.725116 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.253216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10234 2023-05-31 10:23:39.261216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16741 2023-05-31 10:23:23.121118 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.261216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-05-31 10:23:39.261216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-05-31 10:23:23.317119 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-05-31 10:23:39.265216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    10604 2023-05-31 10:23:39.257216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    13410 2023-05-31 10:23:22.921117 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.257216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-31 10:23:39.281216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-31 10:23:38.557212 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.281216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-31 10:23:39.281216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-31 10:23:38.773213 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-31 10:23:39.285216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-31 10:23:39.285216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-31 10:23:25.093130 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.285216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-31 10:23:39.289216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-31 10:23:25.289131 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-31 10:23:39.289216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-31 10:23:39.289216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-31 10:23:25.481132 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.293216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-31 10:23:39.297216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-31 10:23:26.273137 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.297216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-31 10:23:39.293216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-31 10:23:26.077136 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-31 10:23:39.293216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-31 10:23:39.297216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-31 10:23:26.469138 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.301216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-31 10:23:39.265216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-31 10:23:23.521121 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.265216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-31 10:23:39.269216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-31 10:23:23.721122 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.269216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-31 10:23:39.269216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-31 10:23:23.925123 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-31 10:23:39.273216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-31 10:23:39.273216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-31 10:23:24.121124 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.273216 qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-31 10:23:39.425217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-31 10:23:37.281204 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.425217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-31 10:23:39.429217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-31 10:23:37.493205 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-31 10:23:39.429217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-31 10:23:39.429217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-31 10:23:37.693206 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.429217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-31 10:23:39.433217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-31 10:23:37.901208 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-31 10:23:39.433217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-31 10:23:39.433217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-31 10:23:38.121209 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-31 10:23:39.437217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-31 10:23:39.437217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-31 10:23:38.345210 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.437217 qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-31 10:23:39.353217 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-31 10:23:30.773165 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.353217 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-31 10:23:39.353217 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-31 10:23:30.973166 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-31 10:23:39.357216 qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-31 10:23:39.221216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-31 10:23:20.481102 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.225216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-31 10:23:39.225216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-31 10:23:20.677103 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.229216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-31 10:23:39.229216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-31 10:23:20.881105 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-31 10:23:39.229216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-31 10:23:39.233216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-31 10:23:21.081106 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.233216 qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-31 10:23:39.325216 qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-31 10:23:28.461151 qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-31 10:23:39.329216 qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-31 10:23:39.357216 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-31 10:23:31.169167 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.357216 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-31 10:23:39.361217 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-31 10:23:31.369168 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-31 10:23:39.361217 qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-31 10:23:39.377217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-31 10:23:32.717176 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.377217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-31 10:23:39.377217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-31 10:23:32.945178 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.377217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-31 10:23:39.381217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-31 10:23:33.193179 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.381217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-31 10:23:39.381217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-31 10:23:33.441181 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.385217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-31 10:23:39.385217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-31 10:23:33.693182 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.385217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-31 10:23:39.389217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-31 10:23:33.925184 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-31 10:23:39.389217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-31 10:23:39.389217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-31 10:23:34.137185 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.393217 qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-31 10:23:39.365217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-31 10:23:31.817171 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.365217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-31 10:23:39.373217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-31 10:23:32.493175 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.373217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-31 10:23:39.369217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-31 10:23:32.037172 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-31 10:23:39.369217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-31 10:23:39.369217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-31 10:23:32.261174 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.373217 qwak_core-0.0.91/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-31 10:23:39.345216 qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-31 10:23:30.121161 qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-31 10:23:39.345216 qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-31 10:23:39.197216 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-31 10:23:20.089100 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-31 10:23:39.197216 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-31 10:23:39.193215 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-31 10:23:19.897099 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.193215 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-31 10:23:39.197216 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-31 10:23:20.281101 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-31 10:23:39.201216 qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-31 10:23:39.341216 qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-31 10:23:29.693158 qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-31 10:23:39.345216 qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-31 10:23:39.361217 qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-31 10:23:31.585169 qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-31 10:23:39.365217 qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-31 10:23:39.189216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-31 10:23:17.757086 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.193215 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-31 10:23:39.189216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-31 10:23:17.553084 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-31 10:23:39.189216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-31 10:23:39.177215 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-31 10:23:16.945081 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.181215 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-31 10:23:39.181215 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-31 10:23:17.141082 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.185216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-31 10:23:39.185216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-31 10:23:17.337083 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-31 10:23:39.185216 qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-31 10:23:39.397217 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-31 10:23:34.585188 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-31 10:23:39.397217 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-31 10:23:39.393217 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-31 10:23:34.373186 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.393217 qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-31 10:23:39.209216 qwak_core-0.0.91/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-31 10:23:19.133094 qwak_core-0.0.91/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.209216 qwak_core-0.0.91/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3044 2023-05-31 10:23:39.213216 qwak_core-0.0.91/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2641 2023-05-31 10:23:19.325095 qwak_core-0.0.91/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 10:23:39.213216 qwak_core-0.0.91/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-31 10:23:41.621230 qwak_core-0.0.91/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-31 10:23:41.621230 qwak_core-0.0.91/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-31 10:21:45.588519 qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-31 10:21:45.592519 qwak_core-0.0.91/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-31 10:21:45.596519 qwak_core-0.0.91/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.91/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.91/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-31 11:35:53.854165 qwak_core-0.0.92/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 11:37:40.930794 qwak_core-0.0.92/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-31 11:37:40.958794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-31 11:37:19.530667 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.958794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-31 11:37:40.954794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-31 11:37:19.142665 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.954794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-31 11:37:40.954794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-31 11:37:19.334666 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.954794 qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-31 11:37:40.946794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-31 11:37:18.590661 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-31 11:37:40.946794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-31 11:37:40.946794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-31 11:37:18.774662 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.950794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-05-31 11:37:40.950794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-05-31 11:37:18.962664 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.950794 qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-31 11:37:40.934794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-31 11:37:18.382660 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-31 11:37:40.934794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-05-31 11:37:40.934794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-05-31 11:37:19.722668 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.934794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-31 11:37:40.938794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-31 11:37:20.098671 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.942794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-31 11:37:40.942794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-31 11:37:20.298672 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-31 11:37:40.942794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-31 11:37:40.938794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-31 11:37:19.910669 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.938794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-31 11:37:40.942794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-31 11:37:20.494673 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.946794 qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-31 11:37:40.986794 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-31 11:37:23.158689 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.990794 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-31 11:37:40.990794 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-31 11:37:23.350690 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-31 11:37:40.990794 qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-31 11:37:41.066794 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-31 11:37:29.162724 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.066794 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-31 11:37:41.066794 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-31 11:37:29.346725 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-31 11:37:41.066794 qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-31 11:37:41.070795 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-31 11:37:30.274731 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-31 11:37:41.070795 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-31 11:37:41.070795 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-31 11:37:30.090730 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.070795 qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-31 11:37:41.074795 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-31 11:37:30.458732 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.074795 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-31 11:37:41.074795 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-31 11:37:30.638733 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-31 11:37:41.078795 qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-31 11:37:41.170795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-31 11:37:38.586780 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.170795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-31 11:37:41.162795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-31 11:37:38.218778 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.166795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-31 11:37:41.166795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-31 11:37:38.398779 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.166795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-31 11:37:41.158795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-31 11:37:37.842775 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-31 11:37:41.162795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-31 11:37:41.162795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-31 11:37:38.034777 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.162795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-31 11:37:41.174795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-31 11:37:39.162783 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.174795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-31 11:37:41.174795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-31 11:37:38.978782 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.174795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-31 11:37:41.170795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-31 11:37:38.794781 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.170795 qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-31 11:37:41.158795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-31 11:37:37.650774 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.158795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-31 11:37:41.154795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-31 11:37:37.270772 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.154795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-31 11:37:41.154795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-31 11:37:37.466773 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-31 11:37:41.158795 qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-31 11:37:41.102795 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-31 11:37:32.550744 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-31 11:37:41.102795 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-31 11:37:41.098795 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-31 11:37:32.346743 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.102795 qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-05-31 11:37:41.090795 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-05-31 11:37:31.962741 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.094795 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-31 11:37:41.094795 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-31 11:37:32.146742 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.094795 qwak_core-0.0.92/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-31 11:37:41.094795 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-31 11:37:32.758746 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-31 11:37:41.098795 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-05-31 11:37:41.098795 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-05-31 11:37:33.198748 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-31 11:37:41.098795 qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-31 11:37:41.110795 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-31 11:37:33.598750 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.110795 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-31 11:37:41.110795 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-31 11:37:33.782752 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-31 11:37:41.114795 qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-31 11:37:41.086795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-31 11:37:31.406737 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.086795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-31 11:37:41.086795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-31 11:37:31.590739 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-31 11:37:41.086795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-31 11:37:41.078795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-31 11:37:31.026735 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.082795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-31 11:37:41.078795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-31 11:37:30.838734 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.078795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-31 11:37:41.082795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-31 11:37:31.222736 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-31 11:37:41.082795 qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-31 11:37:40.978794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-31 11:37:22.198684 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.978794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-31 11:37:40.978794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-31 11:37:22.386685 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.978794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-31 11:37:40.982794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-31 11:37:22.578686 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-31 11:37:40.982794 qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-31 11:37:41.046795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-31 11:37:28.026718 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.046795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-31 11:37:41.042794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-31 11:37:27.846717 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-31 11:37:41.042794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-31 11:37:41.018794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-31 11:37:25.746704 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.018794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-31 11:37:41.014794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-31 11:37:25.542703 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.018794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-31 11:37:41.010794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-31 11:37:24.930699 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.010794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-31 11:37:41.014794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-31 11:37:25.342702 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-31 11:37:41.014794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-31 11:37:41.022794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-31 11:37:25.942705 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.022794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-31 11:37:41.022794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-31 11:37:26.130706 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-31 11:37:41.022794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-31 11:37:41.010794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-31 11:37:25.134701 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.014794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-31 11:37:41.026794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-31 11:37:26.318708 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.026794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10234 2023-05-31 11:37:41.030794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
+-rw-r--r--   0        0        0    16741 2023-05-31 11:37:26.718710 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.030794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3559 2023-05-31 11:37:41.030794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
+-rw-r--r--   0        0        0     1759 2023-05-31 11:37:26.910711 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3608 2023-05-31 11:37:41.034794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10604 2023-05-31 11:37:41.026794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    13410 2023-05-31 11:37:26.522709 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.026794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-31 11:37:41.046795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-31 11:37:40.454791 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.046795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-31 11:37:41.050794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-31 11:37:40.642792 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-31 11:37:41.050794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-31 11:37:41.050794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-31 11:37:28.606721 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.054794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-31 11:37:41.054794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-31 11:37:28.794722 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-31 11:37:41.054794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-31 11:37:41.054794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-31 11:37:28.978723 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.058795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-31 11:37:41.058795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-31 11:37:29.726728 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.062795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-31 11:37:41.058795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-31 11:37:29.530727 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-31 11:37:41.058795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-31 11:37:41.062795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-31 11:37:29.906729 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.062795 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-31 11:37:41.034794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-31 11:37:27.106712 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.034794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-31 11:37:41.034794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-31 11:37:27.290713 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.038794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-31 11:37:41.038794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-31 11:37:27.474714 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-31 11:37:41.038794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-31 11:37:41.042794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-31 11:37:27.662716 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.042794 qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-31 11:37:41.178795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-31 11:37:39.346784 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.178795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-31 11:37:41.178795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-31 11:37:39.526785 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-31 11:37:41.182795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-31 11:37:41.182795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-31 11:37:39.710787 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.182795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-31 11:37:41.182795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-31 11:37:39.902788 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-31 11:37:41.186795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-31 11:37:41.186795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-31 11:37:40.090789 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-31 11:37:41.186795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-31 11:37:41.186795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-31 11:37:40.274790 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.190795 qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-31 11:37:41.114795 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-31 11:37:33.962753 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.114795 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-31 11:37:41.114795 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-31 11:37:34.142754 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-31 11:37:41.118795 qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-31 11:37:40.994794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-31 11:37:24.174695 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.994794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-31 11:37:40.998794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-31 11:37:24.370696 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.998794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-31 11:37:41.002794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-31 11:37:24.554697 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-31 11:37:41.002794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-31 11:37:41.006794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-31 11:37:24.738698 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.006794 qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-31 11:37:41.090795 qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-31 11:37:31.774740 qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-31 11:37:41.090795 qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-31 11:37:41.118795 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-31 11:37:34.322755 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.118795 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-31 11:37:41.118795 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-31 11:37:34.502756 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-31 11:37:41.122795 qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-31 11:37:41.134795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-31 11:37:35.590762 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.134795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-31 11:37:41.134795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-31 11:37:35.774763 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.138795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-31 11:37:41.138795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-31 11:37:35.962764 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.138795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-31 11:37:41.138795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-31 11:37:36.146766 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.142795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-31 11:37:41.142795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-31 11:37:36.338767 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.142795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-31 11:37:41.142795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-31 11:37:36.542768 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-31 11:37:41.146795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-31 11:37:41.146795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-31 11:37:36.726769 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.146795 qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-31 11:37:41.126795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-31 11:37:34.866758 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.126795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-31 11:37:41.130795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-31 11:37:35.410761 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.130795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-31 11:37:41.126795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-31 11:37:35.046759 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-31 11:37:41.126795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-31 11:37:41.130795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-31 11:37:35.230760 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.130795 qwak_core-0.0.92/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-31 11:37:41.106795 qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-31 11:37:33.406749 qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-31 11:37:41.106795 qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-31 11:37:40.974794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-31 11:37:23.754693 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-31 11:37:40.974794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-31 11:37:40.970794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-31 11:37:23.550691 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.970794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-31 11:37:40.974794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-31 11:37:23.966694 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-31 11:37:40.974794 qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-31 11:37:41.106795 qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-31 11:37:32.970747 qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-31 11:37:41.106795 qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-31 11:37:41.122795 qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-31 11:37:34.682757 qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-31 11:37:41.122795 qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-31 11:37:40.966794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-31 11:37:21.450679 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.970794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-31 11:37:40.966794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-31 11:37:21.258678 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-31 11:37:40.966794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-31 11:37:40.958794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-31 11:37:20.686674 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.958794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-31 11:37:40.962794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-31 11:37:20.874675 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.962794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-31 11:37:40.962794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-31 11:37:21.058677 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-31 11:37:40.966794 qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-31 11:37:41.150795 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-31 11:37:37.090771 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-31 11:37:41.150795 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-31 11:37:41.150795 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-31 11:37:36.906770 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:41.150795 qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-31 11:37:40.982794 qwak_core-0.0.92/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-31 11:37:22.770687 qwak_core-0.0.92/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.986794 qwak_core-0.0.92/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3044 2023-05-31 11:37:40.986794 qwak_core-0.0.92/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2641 2023-05-31 11:37:22.966688 qwak_core-0.0.92/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 11:37:40.986794 qwak_core-0.0.92/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-31 11:37:42.746805 qwak_core-0.0.92/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-31 11:37:42.746805 qwak_core-0.0.92/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    15319 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-31 11:35:53.858165 qwak_core-0.0.92/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-31 11:35:53.862165 qwak_core-0.0.92/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-31 11:35:53.890165 qwak_core-0.0.92/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-31 11:35:53.894165 qwak_core-0.0.92/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.92/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.92/PKG-INFO
```

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.92/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.92/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/pyproject.toml` & `qwak_core-0.0.92/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.91"
+version = "0.0.92"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.91/qwak/automations/__init__.py` & `qwak_core-0.0.92/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/automations/automation_executions.py` & `qwak_core-0.0.92/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/automations/automations.py` & `qwak_core-0.0.92/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.92/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.92/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/automations/common.py` & `qwak_core-0.0.92/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.92/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.92/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.92/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.92/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.92/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/alert_management/client.py` & `qwak_core-0.0.92/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/analytics/client.py` & `qwak_core-0.0.92/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/audience/client.py` & `qwak_core-0.0.92/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/automation_management/client.py` & `qwak_core-0.0.92/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.92/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.92/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.92/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.92/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/build_management/client.py` & `qwak_core-0.0.92/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.92/qwak/clients/build_orchestrator/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,16 @@
 )
 from _qwak_proto.qwak.build.v1.build_api_pb2_grpc import BuildAPIStub
 from _qwak_proto.qwak.build.v1.build_pb2 import BuildFilter, BuildStatus, ModelSchema
 from _qwak_proto.qwak.builds.build_pb2 import (
     BuildEnv,
     BuildProperties,
     BuildPropertiesV1,
-    CpuResources,
     DataTableDefinition,
     DockerEnv,
-    GpuResources,
     MemoryUnit,
     ModelUriSpec,
     PythonEnv,
     RemoteBuildSpec,
 )
 from _qwak_proto.qwak.builds.build_url_pb2 import BuildVersioningUrlParams
 from _qwak_proto.qwak.builds.builds_orchestrator_service_pb2 import (
@@ -47,14 +45,19 @@
     GetBuildVersioningDownloadURLResponse,
     GetBuildVersioningUploadURLRequest,
     GetBuildVersioningUploadURLResponse,
 )
 from _qwak_proto.qwak.builds.builds_orchestrator_service_pb2_grpc import (
     BuildsOrchestratorServiceStub,
 )
+from _qwak_proto.qwak.user_application.common.v0.resources_pb2 import (
+    CpuResources,
+    GpuResources,
+    PodComputeResourceTemplateSpec,
+)
 from dependency_injector.wiring import Provide
 from qwak.exceptions import QwakException
 from qwak.inner.di_configuration import QwakContainer
 from qwak.inner.tool.grpc.grpc_try_wrapping import grpc_try_catch_wrapper
 from yaml import Loader
 
 
@@ -353,23 +356,29 @@
                     qwak_sdk_version_url=qwak_sdk_version_url,
                 ),
                 build_v1_flag=build_v1_flag,
                 build_steps=build_steps,
             )
         )
 
-        if build_conf.build_env.remote.resources.gpu_type:
-            request.build_spec.gpu_resources.CopyFrom(
+        if build_conf.build_env.remote.resources.instance:
+            request.build_spec.client_pod_compute_resources.template_spec.CopyFrom(
+                PodComputeResourceTemplateSpec(
+                    template_id=build_conf.build_env.remote.resources.instance
+                )
+            )
+        elif build_conf.build_env.remote.resources.gpu_type:
+            request.build_spec.client_pod_compute_resources.gpu_resources.CopyFrom(
                 GpuResources(
                     gpu_type=build_conf.build_env.remote.resources.gpu_type,
                     gpu_amount=build_conf.build_env.remote.resources.gpu_amount,
                 )
             )
         else:
-            request.build_spec.cpu_resources.CopyFrom(
+            request.build_spec.client_pod_compute_resources.cpu_resources.CopyFrom(
                 CpuResources(
                     cpu=build_conf.build_env.remote.resources.cpus,
                     memory_amount=int(
                         re.sub(
                             r"\D",
                             "",
                             build_conf.build_env.remote.resources.memory,
@@ -383,15 +392,15 @@
 
         return request
 
     def cancel_build_model(self, build_id: str):
         """cancel remote build process
 
         Args:
-            build_id: The build Id to cancel
+            build_id: The build ID to cancel
 
         Raises:
             QwakException: In case of failing to connect the service
         """
         try:
             self._builds_orchestrator_stub.CancelBuildModel(
                 CancelBuildModelRequest(build_id=build_id)
```

### Comparing `qwak_core-0.0.91/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.92/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/deployment/client.py` & `qwak_core-0.0.92/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.92/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.92/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.92/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.92/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/instance_template/client.py` & `qwak_core-0.0.92/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.92/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/logging_client/client.py` & `qwak_core-0.0.92/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/model_management/client.py` & `qwak_core-0.0.92/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/project/client.py` & `qwak_core-0.0.92/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/secret_service/client.py` & `qwak_core-0.0.92/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.92/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.92/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.92/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.92/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.92/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.92/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.92/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.92/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.92/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.92/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/offline/client.py` & `qwak_core-0.0.92/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/feature_store/online/client.py` & `qwak_core-0.0.92/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/const.py` & `qwak_core-0.0.92/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.92/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.92/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.92/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.92/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/singleton_meta.py` & `qwak_core-0.0.92/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/tool/auth.py` & `qwak_core-0.0.92/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.92/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.92/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.92/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.92/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/__init__.py` & `qwak_core-0.0.92/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.92/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.92/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.92/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.92/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.92/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/base.py` & `qwak_core-0.0.92/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/decorators/api.py` & `qwak_core-0.0.92/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.92/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/experiment_tracking.py` & `qwak_core-0.0.92/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/schema.py` & `qwak_core-0.0.92/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/schema_entities.py` & `qwak_core-0.0.92/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.92/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.92/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.92/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.92/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.92/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.92/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.92/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.92/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/client.py` & `qwak_core-0.0.92/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.92/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/models/model.py` & `qwak_core-0.0.92/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.92/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.92/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/tools/logger/logger.py` & `qwak_core-0.0.92/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak/tools/logger/logging.yml` & `qwak_core-0.0.92/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.92/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/qwak_services_mock/services_mock.py` & `qwak_core-0.0.92/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.91/setup.py` & `qwak_core-0.0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.91',
+    'version': '0.0.92',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.91/PKG-INFO` & `qwak_core-0.0.92/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.91
+Version: 0.0.92
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

