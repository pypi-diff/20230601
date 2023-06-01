# Comparing `tmp/fovus-1.0.4-py3-none-any.whl.zip` & `tmp/fovus-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,26 @@
-Zip file size: 44119 bytes, number of entries: 46
+Zip file size: 47507 bytes, number of entries: 47
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 23-Apr-05 06:40 fovus/root_config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/adapter/__init__.py
 -rw-r--r--  2.0 unx     3331 b- defN 23-Apr-05 06:40 fovus/adapter/aws_cognito_adapter.py
--rw-r--r--  2.0 unx    10856 b- defN 23-Apr-12 04:12 fovus/adapter/fovus_api_adapter.py
+-rw-r--r--  2.0 unx    19085 b- defN 23-Jun-01 05:54 fovus/adapter/fovus_api_adapter.py
 -rw-r--r--  2.0 unx     8700 b- defN 23-May-25 22:01 fovus/adapter/fovus_s3_adapter.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/cli/__init__.py
--rw-r--r--  2.0 unx    13184 b- defN 23-Apr-05 06:40 fovus/cli/cli_action_runner.py
+-rw-r--r--  2.0 unx    13450 b- defN 23-Jun-01 05:54 fovus/cli/cli_action_runner.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Apr-05 06:56 fovus/cli/documenter.py
 -rw-r--r--  2.0 unx      475 b- defN 23-Apr-05 06:40 fovus/cli/fovus_cli.py
--rw-r--r--  2.0 unx    25901 b- defN 23-May-15 05:07 fovus/cli/fovus_cli_argument_parser.py
+-rw-r--r--  2.0 unx    25911 b- defN 23-Jun-01 05:54 fovus/cli/fovus_cli_argument_parser.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/config/__init__.py
--rw-r--r--  2.0 unx      138 b- defN 23-May-25 22:01 fovus/config/config.py
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-01 05:56 fovus/config/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/constants/__init__.py
+-rw-r--r--  2.0 unx     1278 b- defN 23-Jun-01 05:54 fovus/constants/benchmark_constants.py
 -rw-r--r--  2.0 unx       59 b- defN 23-Apr-05 06:40 fovus/constants/cli_action_runner_constants.py
--rw-r--r--  2.0 unx     8641 b- defN 23-May-15 05:17 fovus/constants/cli_constants.py
--rw-r--r--  2.0 unx     1446 b- defN 23-Apr-05 06:40 fovus/constants/fovus_api_constants.py
+-rw-r--r--  2.0 unx     8682 b- defN 23-Jun-01 05:54 fovus/constants/cli_constants.py
+-rw-r--r--  2.0 unx     2100 b- defN 23-Jun-01 05:54 fovus/constants/fovus_api_constants.py
 -rw-r--r--  2.0 unx      194 b- defN 23-Apr-05 06:40 fovus/constants/util_constants.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/exception/__init__.py
 -rw-r--r--  2.0 unx      291 b- defN 23-Apr-05 06:40 fovus/exception/status_code_exception.py
 -rw-r--r--  2.0 unx      183 b- defN 23-Apr-05 06:40 fovus/exception/system_exception.py
 -rw-r--r--  2.0 unx      174 b- defN 23-Apr-05 06:40 fovus/exception/user_exception.py
 -rw-r--r--  2.0 unx     1054 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json
 -rw-r--r--  2.0 unx     1112 b- defN 23-May-15 05:07 fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json
@@ -28,21 +29,21 @@
 -rw-r--r--  2.0 unx       42 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/FOVUS_user_config_template.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/fovus_provided_configs/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/schema/__init__.py
 -rw-r--r--  2.0 unx    10183 b- defN 23-May-15 05:07 fovus/schema/create_job_schema.json
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/util/__init__.py
 -rw-r--r--  2.0 unx     3389 b- defN 23-Apr-05 06:40 fovus/util/aws_util.py
 -rw-r--r--  2.0 unx      334 b- defN 23-Apr-05 06:40 fovus/util/cli_action_runner_util.py
--rw-r--r--  2.0 unx     4616 b- defN 23-May-25 22:01 fovus/util/file_util.py
--rw-r--r--  2.0 unx     2871 b- defN 23-Apr-05 06:40 fovus/util/fovus_api_util.py
+-rw-r--r--  2.0 unx     4625 b- defN 23-Jun-01 05:54 fovus/util/file_util.py
+-rw-r--r--  2.0 unx     7357 b- defN 23-Jun-01 05:54 fovus/util/fovus_api_util.py
 -rw-r--r--  2.0 unx     1740 b- defN 23-Apr-05 06:40 fovus/util/fovus_cli_argument_parser_util.py
 -rw-r--r--  2.0 unx     1519 b- defN 23-Apr-05 06:40 fovus/util/fovus_s3_adapter_util.py
 -rw-r--r--  2.0 unx      533 b- defN 23-Apr-05 06:40 fovus/util/util.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-05 06:40 fovus/validator/__init__.py
--rw-r--r--  2.0 unx     3935 b- defN 23-May-12 19:25 fovus/validator/fovus_api_validator.py
--rw-r--r--  2.0 unx    14101 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     8883 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       51 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4089 b- defN 23-May-25 22:02 fovus-1.0.4.dist-info/RECORD
-46 files, 134363 bytes uncompressed, 37463 bytes compressed:  72.1%
+-rw-r--r--  2.0 unx     3732 b- defN 23-Jun-01 05:54 fovus/validator/fovus_api_validator.py
+-rw-r--r--  2.0 unx    14101 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     8883 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       51 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4184 b- defN 23-Jun-01 05:58 fovus-1.0.5.dist-info/RECORD
+47 files, 149228 bytes uncompressed, 40699 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -36,14 +36,17 @@
 
 Filename: fovus/config/config.py
 Comment: 
 
 Filename: fovus/constants/__init__.py
 Comment: 
 
+Filename: fovus/constants/benchmark_constants.py
+Comment: 
+
 Filename: fovus/constants/cli_action_runner_constants.py
 Comment: 
 
 Filename: fovus/constants/cli_constants.py
 Comment: 
 
 Filename: fovus/constants/fovus_api_constants.py
@@ -114,26 +117,26 @@
 
 Filename: fovus/validator/__init__.py
 Comment: 
 
 Filename: fovus/validator/fovus_api_validator.py
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/LICENSE.txt
+Filename: fovus-1.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/METADATA
+Filename: fovus-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/WHEEL
+Filename: fovus-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/entry_points.txt
+Filename: fovus-1.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/top_level.txt
+Filename: fovus-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: fovus-1.0.4.dist-info/RECORD
+Filename: fovus-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fovus/adapter/fovus_api_adapter.py

```diff
@@ -1,88 +1,216 @@
 import copy
 import json
 import os
+from http import HTTPStatus
 
 import requests
 
 from fovus.adapter.aws_cognito_adapter import AwsCognitoAdapter, UserAttribute
+from fovus.constants.benchmark_constants import (
+    BENCHMARK_NAME,
+    BOUNDS,
+    COMPARISONS,
+    COMPREHENSIONS,
+    CORRECTABLE_COMPARISON,
+)
 from fovus.constants.cli_constants import (
+    BENCHMARKING_PROFILE_NAME,
+    COMPUTING_DEVICE,
+    CPU,
+    ENABLE_HYPERTHREADING,
     FOVUS_PROVIDED_CONFIGS,
     JOB_CONFIG_CONTAINERIZED_TEMPLATE,
     JOB_CONFIG_FILE_PATH,
     JOB_NAME,
+    MAX_GPU,
+    MIN_GPU,
+    MIN_GPU_MEM_GIB,
     MONOLITHIC_OVERRIDE,
     PATH_TO_CONFIG_FILE_IN_REPO,
     TIMESTAMP,
     USER_ID,
     WORKSPACE_ID,
 )
 from fovus.constants.fovus_api_constants import (
     APIS,
     AUTHORIZATION_HEADER,
+    BENCHMARK,
     BODY,
-    CONTAINERIZED,
+    BOUND_VALUE_CORRECTION_PRINT_ORDER,
+    BP_HYPERTHREADING,
     CREATE_JOB,
     ENVIRONMENT,
     FILE,
     GET_FILE_DOWNLOAD_TOKEN,
     GET_FILE_UPLOAD_TOKEN,
     GET_JOB_INFO,
     JOB,
     JOB_STATUS,
     LICENSE_COUNT_PER_TASK,
     LICENSE_FEATURE,
+    LIST_BENCHMARK_PROFILE,
     LIST_SOFTWARE,
     MONOLITHIC_LIST,
+    PAYLOAD_CONSTRAINTS,
+    PAYLOAD_JOB_CONSTRAINTS,
     PAYLOAD_JOB_NAME,
+    PAYLOAD_TASK_CONSTRAINTS,
     PAYLOAD_TIMESTAMP,
     PAYLOAD_WORKSPACE_ID,
     SOFTWARE,
+    SOFTWARE_MAP,
     SOFTWARE_NAME,
+    SOFTWARE_VERSION,
+    SOFTWARE_VERSIONS,
     TIMEOUT_SECONDS,
     VENDOR_NAME,
 )
 from fovus.constants.util_constants import UTF8
+from fovus.exception.user_exception import UserException
 from fovus.root_config import ROOT_DIR
 from fovus.util.fovus_api_util import FovusApiUtil
-from fovus.validator.fovus_api_validator import FovusApiValidator
 
 
 class FovusApiAdapter:
     def __init__(self, auth_type, auth_parameters, client_id):
         self.cognito_adapter = AwsCognitoAdapter()
         self.cognito_adapter.authenticate(auth_type, auth_parameters, client_id)
 
     def create_job(self, request):
-        request = self._fill_missing_vendor_names(request)
         headers = self._get_api_authorization_header()
         response = requests.post(APIS[JOB][CREATE_JOB], json=request, headers=headers, timeout=TIMEOUT_SECONDS)
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
-    def _fill_missing_vendor_names(self, create_job_request):
-        print("Attempting to fill missing/empty vendorName fields (if needed)...")
-        if MONOLITHIC_LIST in create_job_request[ENVIRONMENT]:
-            list_software_response = {}
-            monolithic_list_copy = copy.deepcopy(create_job_request[ENVIRONMENT][MONOLITHIC_LIST])
-            for i, monolithic_list_item in enumerate(monolithic_list_copy):
-                if FovusApiUtil.should_fill_vendor_name(monolithic_list_item):
-                    if not list_software_response:
-                        list_software_response = self.list_software()
-                    vendor_name = FovusApiUtil.get_software_vendor(
-                        list_software_response, monolithic_list_item[SOFTWARE_NAME]
-                    )
-                    create_job_request[ENVIRONMENT][MONOLITHIC_LIST][i][VENDOR_NAME] = vendor_name
-                    print(
-                        f"Filled name for {SOFTWARE_NAME} {monolithic_list_item[SOFTWARE_NAME]} "
-                        + f"with {VENDOR_NAME} {vendor_name}"
-                    )
-        elif CONTAINERIZED in create_job_request[ENVIRONMENT]:
+    def make_dynamic_changes_to_create_job_request(self, request):
+        self._make_dynamic_changes_to_software(request)
+        self._validate_benchmarking_profile(request)
+
+    def _make_dynamic_changes_to_software(self, request):
+        print("Validating software...")
+        if MONOLITHIC_LIST not in request[ENVIRONMENT]:
             print("Request is for a containerized job. Filling missing/empty vendorName fields is not required.")
-        return create_job_request
+            return
+
+        list_software_response = self.list_software()
+        for i, monolithic_list_item in enumerate(copy.deepcopy(request[ENVIRONMENT][MONOLITHIC_LIST])):
+            software_name = monolithic_list_item[SOFTWARE_NAME]
+            software_version = monolithic_list_item[SOFTWARE_VERSION]
+            software_vendor = monolithic_list_item[VENDOR_NAME]
+
+            valid_software_names = []
+            is_valid_software_name = False
+            for valid_software_vendor in list_software_response[SOFTWARE_MAP]:
+                if software_name in list_software_response[SOFTWARE_MAP][valid_software_vendor]:
+                    is_valid_software_name = True
+                    if (
+                        software_version
+                        in list_software_response[SOFTWARE_MAP][valid_software_vendor][software_name][SOFTWARE_VERSIONS]
+                    ):
+                        if valid_software_vendor != software_vendor:
+                            print(
+                                f"Replacing vendor name '{software_vendor}' with "
+                                f"'{valid_software_vendor}' for monolithic list item {monolithic_list_item}."
+                            )
+                            request[ENVIRONMENT][MONOLITHIC_LIST][i][VENDOR_NAME] = valid_software_vendor
+                        break  # Successful validation of current list item.
+                    raise UserException(
+                        HTTPStatus.BAD_REQUEST,
+                        self.__class__.__name__,
+                        f"Software version '{software_version}' for software name '{software_name}' is not valid. "
+                        + "Valid software versions: "
+                        + str(
+                            list_software_response[SOFTWARE_MAP][valid_software_vendor][software_name][
+                                SOFTWARE_VERSIONS
+                            ]
+                        ),
+                    )
+                valid_software_names.append(
+                    {valid_software_vendor: list(list_software_response[SOFTWARE_MAP][valid_software_vendor].keys())}
+                )
+            if not is_valid_software_name:
+                raise UserException(
+                    HTTPStatus.BAD_REQUEST,
+                    self.__class__.__name__,
+                    f"Software name '{software_name}' is not valid. "
+                    + "Valid software vendors and names (format: [{vendor: [name, ...]}, ...]): "
+                    + str(valid_software_names),
+                )
+
+    def _validate_benchmarking_profile(self, request):  # pylint: disable=too-many-locals
+        benchmarking_profile_name = request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][BENCHMARKING_PROFILE_NAME]
+        hyperthreading_enabled = request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][ENABLE_HYPERTHREADING]
+        print(
+            f"Validating the benchmarking profile '{benchmarking_profile_name}' and "
+            "updating values if necessary and possible..."
+        )
+        list_benchmark_profile_response = self.list_benchmarking_profile(request[PAYLOAD_WORKSPACE_ID])
+        valid_benchmarking_profile_names = []
+        for current_benchmarking_profile in list_benchmark_profile_response[  # pylint: disable=too-many-nested-blocks
+            BODY
+        ]:
+            current_benchmarking_profile_name = current_benchmarking_profile[BENCHMARK_NAME]
+            valid_benchmarking_profile_names.append(current_benchmarking_profile_name)
+            if benchmarking_profile_name == current_benchmarking_profile_name:
+                validations_config = FovusApiUtil.get_benchmark_validations_config(request)
+                bound_scaler = FovusApiUtil.get_benchmark_bound_scaler(
+                    hyperthreading_enabled,
+                    current_benchmarking_profile[BP_HYPERTHREADING],
+                )
+                FovusApiUtil.print_benchmark_hyperthreading_info(hyperthreading_enabled)
+                corrected_value_messages = {}
+                for validation_type in validations_config:  # pylint: disable=consider-using-dict-items
+                    for bound_to_validate in validations_config[validation_type][BOUNDS]:
+                        current_value = request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][bound_to_validate]
+                        benchmarking_profile_bounds = FovusApiUtil.get_benchmark_profile_bounds(
+                            current_benchmarking_profile, bound_to_validate, bound_scaler
+                        )
+                        for comparison, comprehension in zip(COMPARISONS, COMPREHENSIONS):
+                            if comparison in validations_config[validation_type]:
+                                benchmarking_profile_item_bound = validations_config[validation_type][comprehension](
+                                    benchmarking_profile_bounds
+                                )
+                                if validations_config[validation_type][comparison](
+                                    current_value, benchmarking_profile_item_bound
+                                ):
+                                    if comparison == CORRECTABLE_COMPARISON:
+                                        corrected_value_messages[
+                                            bound_to_validate
+                                        ] = FovusApiUtil.get_corrected_value_message(
+                                            validation_type,
+                                            benchmarking_profile_name,
+                                            bound_to_validate,
+                                            benchmarking_profile_item_bound,
+                                            hyperthreading_enabled,
+                                            current_value,
+                                        )
+                                        request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][
+                                            bound_to_validate
+                                        ] = benchmarking_profile_item_bound
+                                    else:
+                                        raise UserException(
+                                            HTTPStatus.BAD_REQUEST,
+                                            self.__class__.__name__,
+                                            f"Invalid value of {current_value} for {bound_to_validate} with "
+                                            f"benchmarking profile {benchmarking_profile_name}. "
+                                            f"Allowed range: "
+                                            f"[{min(benchmarking_profile_bounds)}, {max(benchmarking_profile_bounds)}]",
+                                        )
+                for bound_value_correction in BOUND_VALUE_CORRECTION_PRINT_ORDER:
+                    if bound_value_correction in corrected_value_messages:
+                        print(corrected_value_messages[bound_value_correction])
+                return  # Successful validation.
+
+        raise UserException(
+            HTTPStatus.BAD_REQUEST,
+            self.__class__.__name__,
+            f"Invalid benchmarking profile: '{benchmarking_profile_name}'. "
+            + f"Valid benchmarking profiles: {valid_benchmarking_profile_names}",
+        )
 
     def get_file_download_token(self, request):
         headers = self._get_api_authorization_header()
         response = requests.post(
             APIS[FILE][GET_FILE_DOWNLOAD_TOKEN], json=request, headers=headers, timeout=TIMEOUT_SECONDS
         )
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
@@ -118,30 +246,40 @@
 
     def list_software(self):
         headers = self._get_api_authorization_header()
         response = requests.get(APIS[SOFTWARE][LIST_SOFTWARE], headers=headers, timeout=TIMEOUT_SECONDS)
         FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
         return response.json()
 
+    def list_benchmarking_profile(self, workspace_id):
+        headers = self._get_api_authorization_header()
+        response = requests.get(
+            APIS[BENCHMARK][LIST_BENCHMARK_PROFILE],
+            params={"workspaceId": workspace_id},
+            headers=headers,
+            timeout=TIMEOUT_SECONDS,
+        )
+        FovusApiUtil.confirm_successful_response(response.json(), self.__class__.__name__)
+        return response.json()
+
     def get_user_id(self):
         return self.cognito_adapter.get_user_attribute(UserAttribute.USER_ID)
 
     def _get_api_authorization_header(self):
         return {
             AUTHORIZATION_HEADER: self.cognito_adapter.get_id_token(),
         }
 
     @staticmethod
     def get_create_job_request(cli_dict):
         with open(os.path.expanduser(cli_dict[JOB_CONFIG_FILE_PATH]), encoding=UTF8) as job_config_file:
             create_job_request = json.load(job_config_file)
             FovusApiAdapter._add_create_job_request_remaining_fields(create_job_request, cli_dict)
             FovusApiAdapter._apply_cli_overrides_to_request(create_job_request, cli_dict)
-            FovusApiValidator.validate(create_job_request, CREATE_JOB)
-            FovusApiValidator.validate_additional_create_job_fields(create_job_request)
+            FovusApiAdapter._apply_computing_device_overrides(create_job_request)
             return create_job_request
 
     @staticmethod
     def _add_create_job_request_remaining_fields(create_job_request, cli_dict):
         create_job_request[PAYLOAD_TIMESTAMP] = cli_dict[TIMESTAMP]
         create_job_request[PAYLOAD_WORKSPACE_ID] = cli_dict[WORKSPACE_ID]
         if cli_dict.get(JOB_NAME):
@@ -219,13 +357,28 @@
                     f"{sub_dict.get(sub_dict_parameter_key)} with {cli_dict[sub_dict_parameter_key]}."
                 )
                 if isinstance(cli_dict_value, str) and cli_dict_value.isdigit():
                     cli_dict_value = int(cli_dict_value)
                 sub_dict[sub_dict_parameter_key] = cli_dict_value
 
     @staticmethod
+    def _apply_computing_device_overrides(create_job_request):
+        value_was_overridden = False
+        computing_device = create_job_request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][COMPUTING_DEVICE]
+        print(f"Computing device is {computing_device}. Overriding related constraints if needed...")
+        if computing_device == CPU:
+            for field in [MIN_GPU, MAX_GPU, MIN_GPU_MEM_GIB]:
+                current_field_value = create_job_request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][field]
+                if current_field_value != 0:
+                    print(f"Overriding current {field} value of {current_field_value} with 0.")
+                    value_was_overridden = True
+                    create_job_request[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][field] = 0
+        if not value_was_overridden:
+            print("No overrides necessary.")
+
+    @staticmethod
     def get_file_upload_download_token_request(cli_dict, duration_seconds=3600):
         return {"workspaceId": cli_dict["workspace_id"], "durationSeconds": duration_seconds}
 
     @staticmethod
     def get_job_info_request(cli_dict, job_id):
         return {"workspaceId": cli_dict["workspace_id"], "jobId": job_id}
```

## fovus/cli/cli_action_runner.py

```diff
@@ -29,23 +29,24 @@
     UNIX_OPEN,
     USER_CONFIG_TEMPLATE_FILE_NAME,
     USER_ID,
     USERNAME,
     WINDOWS_EXPLORER,
     WORKSPACE_ID,
 )
-from fovus.constants.fovus_api_constants import PAYLOAD_WORKSPACE_ID
+from fovus.constants.fovus_api_constants import CREATE_JOB, PAYLOAD_WORKSPACE_ID
 from fovus.constants.util_constants import UTF8
 from fovus.exception.status_code_exception import StatusException
 from fovus.exception.user_exception import UserException
 from fovus.root_config import ROOT_DIR
 from fovus.util.cli_action_runner_util import CliActionRunnerUtil
 from fovus.util.file_util import FOVUS_JOB_INFO_FOLDER
 from fovus.util.fovus_api_util import FovusApiUtil
 from fovus.util.util import Util
+from fovus.validator.fovus_api_validator import FovusApiValidator
 
 
 class CliActionRunner:  # pylint: disable=too-few-public-methods
     def __init__(self, args_dict):
         self.args_dict = args_dict
 
     def run_actions(self):
@@ -243,14 +244,17 @@
         )
         self._try_set_user_id(fovus_api_adapter)
         fovus_s3_adapter = FovusS3Adapter(fovus_api_adapter, self.args_dict, self.args_dict[JOB_FILE_ROOT_DIRECTORY])
         print(GENERIC_SUCCESS)
 
         print("Creating and validating create job request...")
         create_job_request = FovusApiAdapter.get_create_job_request(self.args_dict)
+        fovus_api_adapter.make_dynamic_changes_to_create_job_request(create_job_request)
+        validator = FovusApiValidator(create_job_request, CREATE_JOB)
+        validator.validate()
         print(GENERIC_SUCCESS)
 
         fovus_s3_adapter.upload_files()
 
         print("Creating job...")
         fovus_api_adapter.create_job(create_job_request)
         print(GENERIC_SUCCESS)
```

## fovus/cli/fovus_cli_argument_parser.py

```diff
@@ -5,21 +5,23 @@
 
 from fovus.constants.cli_constants import (
     BENCHMARKING_PROFILE_NAME,
     BOOLEAN_ARGS,
     CLI_ARGUMENTS,
     COMPUTING_DEVICE,
     CONFIGURE,
+    CPU,
     CREATE_JOB_WITH_UPLOAD,
     DEFAULT_USER_CONFIG_FILE_PATH,
     DOWNLOAD_JOB_FILES,
     ENABLE_HYPERTHREADING,
     EXCLUDE_INPUT,
     EXCLUDE_OUTPUT,
     GET_JOB_CURRENT_STATUS,
+    GPU,
     INCLUDE_INPUT,
     INCLUDE_OUTPUT,
     IS_SUBJECT_TO_AVAILABLE_RESOURCES,
     JOB_CONFIG_FILE_PATH,
     JOB_FILE_ROOT_DIRECTORY,
     JOB_ID,
     JOB_NAME,
@@ -245,15 +247,15 @@
             + USED_FOR_OVERRIDING_JOB_CONFIG_VALUES,
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[COMPUTING_DEVICE],
             dest=COMPUTING_DEVICE,
             default=None,
             type=str,
-            choices=["cpu", "cpu+gpu"],
+            choices=[CPU, GPU],
             help=f"The target computing device(s) for running your workload. {USED_FOR_OVERRIDING_JOB_CONFIG_VALUES}",
         )
         self.parser.add_argument(
             *CLI_ARGUMENTS[JOB_NAME],
             dest=JOB_NAME,
             default=None,
             type=str,
```

## fovus/constants/cli_constants.py

```diff
@@ -125,14 +125,18 @@
         DOWNLOAD_JOB_FILES,
         GET_JOB_CURRENT_STATUS,
     ),
     (INCLUDE_INPUT, EXCLUDE_INPUT),
     (INCLUDE_OUTPUT, EXCLUDE_OUTPUT),
 ]
 
+# Job types
+CPU = "cpu"
+GPU = "cpu+gpu"
+
 PASSWORD_ENVIRONMENT_VARIABLE_KEY = "FOVUS_CLI_PASSWORD"  # nosec
 PATH_TO_CONFIG_ROOT = os.path.join(os.path.expanduser("~"), ".fovus")
 PATH_TO_JOB_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_configs")
 PATH_TO_USER_CONFIGS = os.path.join(PATH_TO_CONFIG_ROOT, "user_configs")
 PATH_TO_JOB_LOGS = os.path.join(PATH_TO_CONFIG_ROOT, "job_logs")
 UNIX_OPEN = "open"
 WINDOWS_EXPLORER = "explorer"
```

## fovus/constants/fovus_api_constants.py

```diff
@@ -1,37 +1,52 @@
 # API
 from fovus.config.config import DOMAIN_NAME
+from fovus.constants.cli_constants import MAX_VCPU, MIN_VCPU
 
 COGNITO_REGION = "us-east-1"
 TIMEOUT_SECONDS = 10
 
+# API
+JOB = "job"
+FILE = "file"
+SOFTWARE = "software"
+BENCHMARK = "benchmark"
+__APIS = {
+    JOB: DOMAIN_NAME + "/job",
+    FILE: DOMAIN_NAME + "/file",
+    SOFTWARE: DOMAIN_NAME + "/software",
+    BENCHMARK: DOMAIN_NAME + "/benchmark",
+}
+
 CREATE_JOB = "CREATE_JOB"
 GET_JOB_INFO = "GET_JOB_STATUS"
 
 GET_FILE_DOWNLOAD_TOKEN = "GET_FILE_DOWNLOAD_TOKEN"  # nosec
 GET_FILE_UPLOAD_TOKEN = "GET_FILE_UPLOAD_TOKEN"  # nosec
 
 LIST_SOFTWARE = "LIST_SOFTWARE"
 
-FILE = "file"
-JOB = "job"
-SOFTWARE = "software"
+LIST_BENCHMARK_PROFILE = "LIST_BENCHMARK_PROFILE"
 
-__APIS = {JOB: DOMAIN_NAME + "/job"}
 APIS = {
     JOB: {CREATE_JOB: __APIS[JOB] + "/create-job", GET_JOB_INFO: __APIS[JOB] + "/get-job-info"},
     FILE: {
-        GET_FILE_DOWNLOAD_TOKEN: DOMAIN_NAME + "/file/get-file-download-token",
-        GET_FILE_UPLOAD_TOKEN: DOMAIN_NAME + "/file/get-file-upload-token",
+        GET_FILE_DOWNLOAD_TOKEN: __APIS[FILE] + "/get-file-download-token",
+        GET_FILE_UPLOAD_TOKEN: __APIS[FILE] + "/get-file-upload-token",
     },
     SOFTWARE: {
-        LIST_SOFTWARE: DOMAIN_NAME + "/software/list-software",
+        LIST_SOFTWARE: __APIS[SOFTWARE] + "/list-software",
     },
+    BENCHMARK: {LIST_BENCHMARK_PROFILE: __APIS[BENCHMARK] + "/list-benchmark-profile"},
 }
 
+# Benchmarking
+BOUNDS_TO_SCALE = (MIN_VCPU, MAX_VCPU)
+BOUND_VALUE_CORRECTION_PRINT_ORDER = ("minvCpu", "maxvCpu", "minvCpuMemGiB", "minGpu", "maxGpu", "minGpuMemGiB")
+
 # Payload
 AUTHORIZATION_HEADER = "Authorization"
 CONTAINERIZED = "containerized"
 ENVIRONMENT = "environment"
 LICENSE_COUNT_PER_TASK = "licenseCountPerTask"
 LICENSE_FEATURE = "licenseFeature"
 MONOLITHIC_LIST = "monolithicList"
@@ -39,14 +54,18 @@
 PAYLOAD_JOB_CONSTRAINTS = "jobConstraints"
 PAYLOAD_JOB_NAME = "jobName"
 PAYLOAD_TASK_CONSTRAINTS = "taskConstraints"
 PAYLOAD_TIME_COST_PRIORITY_RATIO = "timeToCostPriorityRatio"
 PAYLOAD_TIMESTAMP = "timestamp"
 PAYLOAD_WORKSPACE_ID = "workspaceId"
 SOFTWARE_NAME = "softwareName"
+SOFTWARE_VERSION = "softwareVersion"
 STATUS_CODE = "statusCode"
 VENDOR_NAME = "vendorName"
 
 # Response
 BODY = "body"
+BP_HYPERTHREADING = "bpHyperthreading"
 ERROR_MESSAGE = "errorMessage"
 JOB_STATUS = "jobStatus"
+SOFTWARE_MAP = "softwareMap"
+SOFTWARE_VERSIONS = "softwareVersions"
```

## fovus/util/file_util.py

```diff
@@ -38,15 +38,15 @@
         return local_filepath_list, len(task_directories), total_file_size_bytes
 
     @staticmethod
     def _get_directories_in_directory(root_directory_path, include_input_list, exclude_input_list):
         directories = []
         for entry in os.scandir(root_directory_path):
             if entry.is_dir() and FileUtil.include_exclude_allows_path(
-                entry.name, include_input_list, exclude_input_list
+                entry.name + os.sep, include_input_list, exclude_input_list
             ):
                 directories.append(entry.name)
         return directories
 
     @staticmethod
     def should_ignore_path(file_name):
         if FileUtil._path_contains_directory(file_name, FOVUS_JOB_INFO_FOLDER):
```

## fovus/util/fovus_api_util.py

```diff
@@ -1,13 +1,39 @@
+import operator
 from http import HTTPStatus
 
 import boto3
 
-from fovus.constants.cli_constants import JOB_ID, TIMESTAMP, USER_ID
-from fovus.constants.fovus_api_constants import ERROR_MESSAGE, STATUS_CODE
+from fovus.constants.benchmark_constants import (
+    BOUNDS,
+    CORRECTABLE_COMPARISON,
+    CORRECTABLE_LIST_COMPREHENSION,
+    DEFAULT_BOOLEANS_TO_VALIDATE,
+    DEFAULT_LOWER_BOUNDS_TO_VALIDATE,
+    DEFAULT_UPPER_BOUNDS_TO_VALIDATE,
+    GPU_LOWER_BOUNDS_TO_VALIDATE,
+    GPU_UPPER_BOUNDS_TO_VALIDATE,
+    INCORRECTABLE_COMPARISON,
+    INCORRECTABLE_LIST_COMPREHENSION,
+    LIST_BENCHMARKING_FIELD_BY_CREATE_JOB_REQUEST_FIELD,
+)
+from fovus.constants.cli_constants import (
+    COMPUTING_DEVICE,
+    GPU,
+    JOB_ID,
+    TIMESTAMP,
+    USER_ID,
+)
+from fovus.constants.fovus_api_constants import (
+    BOUNDS_TO_SCALE,
+    ERROR_MESSAGE,
+    PAYLOAD_CONSTRAINTS,
+    PAYLOAD_JOB_CONSTRAINTS,
+    STATUS_CODE,
+)
 from fovus.constants.util_constants import (
     SERVER_ERROR_PREFIX,
     SUCCESS_STATUS_CODES,
     USER_ERROR_PREFIX,
 )
 from fovus.exception.system_exception import SystemException
 from fovus.exception.user_exception import UserException
@@ -65,7 +91,90 @@
             FovusApiUtil.__name__,
             f"Software {software_name} not found in list of available software, unable to retrieve version.",
         )
 
     @staticmethod
     def should_fill_vendor_name(monolithic_list_item):
         return monolithic_list_item.get("softwareName") and not monolithic_list_item.get("vendorName")
+
+    @staticmethod
+    def get_benchmark_validations_config(request):
+        lower_bounds_to_validate = DEFAULT_LOWER_BOUNDS_TO_VALIDATE
+        upper_bounds_to_validate = DEFAULT_UPPER_BOUNDS_TO_VALIDATE
+        boolean_values_to_validate = DEFAULT_BOOLEANS_TO_VALIDATE
+        if request[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][COMPUTING_DEVICE] == GPU:
+            lower_bounds_to_validate.extend(GPU_LOWER_BOUNDS_TO_VALIDATE)
+            upper_bounds_to_validate.extend(GPU_UPPER_BOUNDS_TO_VALIDATE)
+
+        return {
+            "Minimum": {
+                BOUNDS: lower_bounds_to_validate,
+                CORRECTABLE_COMPARISON: operator.lt,
+                CORRECTABLE_LIST_COMPREHENSION: min,
+                INCORRECTABLE_COMPARISON: operator.gt,
+                INCORRECTABLE_LIST_COMPREHENSION: max,
+            },
+            "Maximum": {
+                BOUNDS: upper_bounds_to_validate,
+                CORRECTABLE_COMPARISON: operator.gt,
+                CORRECTABLE_LIST_COMPREHENSION: max,
+                INCORRECTABLE_COMPARISON: operator.lt,
+                INCORRECTABLE_LIST_COMPREHENSION: min,
+            },
+            "Boolean": {
+                BOUNDS: boolean_values_to_validate,
+                CORRECTABLE_COMPARISON: operator.ne,
+                CORRECTABLE_LIST_COMPREHENSION: lambda x: x,
+            },
+        }
+
+    @staticmethod
+    def get_benchmark_profile_bounds(benchmarking_profile_item, bound_to_validate, bound_scaler):
+        benchmarking_profile_bounds = benchmarking_profile_item[
+            LIST_BENCHMARKING_FIELD_BY_CREATE_JOB_REQUEST_FIELD[bound_to_validate]
+        ]
+        # May be list of valid values, dict with "Min" and "Max" keys, or boolean value.
+        if isinstance(benchmarking_profile_bounds, dict):
+            benchmarking_profile_bounds = list(benchmarking_profile_bounds.values())
+        if bound_to_validate in BOUNDS_TO_SCALE:
+            benchmarking_profile_bounds = [int(bound * bound_scaler) for bound in benchmarking_profile_bounds]
+        return benchmarking_profile_bounds
+
+    @staticmethod
+    def get_benchmark_bound_scaler(enable_hyperthreading, bp_hyperthreading):
+        if enable_hyperthreading and bp_hyperthreading:
+            bound_scaler = 1
+        if not enable_hyperthreading and bp_hyperthreading:
+            bound_scaler = 0.5
+        if enable_hyperthreading and not bp_hyperthreading:
+            bound_scaler = 2
+        if not enable_hyperthreading and not bp_hyperthreading:
+            bound_scaler = 1
+        return bound_scaler
+
+    @staticmethod
+    def print_benchmark_hyperthreading_info(enable_hyperthreading):
+        enable_hyperthreading_print = "disabled"
+        threads_per_cpu_message = "1 thread (vCPU) per core can be used on all CPUs."
+        if enable_hyperthreading:
+            enable_hyperthreading_print = "enabled"
+            threads_per_cpu_message = "2 threads (vCPU) per core can be used on CPUs that support hyperthreading."
+        print(f"Hyperthreading is {enable_hyperthreading_print}. {threads_per_cpu_message}")
+
+    @staticmethod
+    def get_corrected_value_message(  # pylint: disable=too-many-arguments
+        validation_type,
+        benchmarking_profile_name,
+        bound_to_validate,
+        benchmarking_profile_item_bound,
+        hyperthreading_enabled,
+        current_value,
+    ):
+        message = (
+            f"{validation_type} value allowed by '{benchmarking_profile_name}' for "
+            f"{bound_to_validate} is {benchmarking_profile_item_bound}"
+        )
+        if bound_to_validate in BOUNDS_TO_SCALE:
+            hyperthreading_enabled_print = "enabled" if hyperthreading_enabled else "disabled"
+            message += f" given that hyperthreading is {hyperthreading_enabled_print}"
+        message += f". Overriding current value of {current_value} with " f"{benchmarking_profile_item_bound}."
+        return message
```

## fovus/validator/fovus_api_validator.py

```diff
@@ -1,20 +1,20 @@
 import json
 import os
 from http import HTTPStatus
 
 import jsonschema
 
 from fovus.constants.cli_constants import (
-    PARALLELISM_OPTIMIZATION,
-    SCALABLE_PARALLELISM,
-    MIN_VCPU,
+    MAX_GPU,
     MAX_VCPU,
     MIN_GPU,
-    MAX_GPU,
+    MIN_VCPU,
+    PARALLELISM_OPTIMIZATION,
+    SCALABLE_PARALLELISM,
 )
 from fovus.constants.fovus_api_constants import (
     PAYLOAD_CONSTRAINTS,
     PAYLOAD_JOB_CONSTRAINTS,
     PAYLOAD_TASK_CONSTRAINTS,
     PAYLOAD_TIME_COST_PRIORITY_RATIO,
 )
@@ -23,78 +23,77 @@
 from fovus.root_config import ROOT_DIR
 
 SCHEMA_PATH_PREFIX = "schema/"
 SCHEMA_PATH_SUFFIX = "_schema.json"
 
 
 class FovusApiValidator:  # pylint: disable=too-few-public-methods
-    @staticmethod
-    def validate(payload, api_method):
+    def __init__(self, payload, api_method):
+        self.payload = payload
+        self.api_method = api_method
+
+    def validate(self):
+        self._validate_schema()
+        self._validate_time_cost_to_priority_ratio()
+        self._validate_parallelism_optimization_allowed_value()
+        self._validate_min_max_vcpu()
+        self._validate_min_max_gpu()
+
+    def _validate_schema(self):
         schema_path = os.path.abspath(
-            os.path.join(ROOT_DIR, SCHEMA_PATH_PREFIX, "".join((api_method.lower(), SCHEMA_PATH_SUFFIX)))
+            os.path.join(ROOT_DIR, SCHEMA_PATH_PREFIX, "".join((self.api_method.lower(), SCHEMA_PATH_SUFFIX)))
         )
         with open(schema_path, encoding=UTF8) as schema_file:
             schema = json.load(schema_file)
             try:
-                jsonschema.validate(payload, schema)
+                jsonschema.validate(self.payload, schema)
             except jsonschema.exceptions.ValidationError as exception:
                 raise UserException(
                     HTTPStatus.BAD_REQUEST.value, FovusApiValidator.__name__, exception.message
                 ) from exception
 
-    @staticmethod
-    def validate_additional_create_job_fields(payload):
-        FovusApiValidator._validate_time_cost_to_priority_ratio(
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][PAYLOAD_TIME_COST_PRIORITY_RATIO]
-        )
-        FovusApiValidator._validate_parallelism_optimization_allowed_value(
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][PARALLELISM_OPTIMIZATION],
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][SCALABLE_PARALLELISM],
-        )
-        FovusApiValidator._validate_min_max_vcpu(
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MIN_VCPU],
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MAX_VCPU],
-        )
-        FovusApiValidator._validate_min_max_gpu(
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MIN_GPU],
-            payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MAX_GPU],
-        )
-
-    @staticmethod
-    def _validate_time_cost_to_priority_ratio(time_cost_to_priority_ratio):
+    def _validate_time_cost_to_priority_ratio(self):
         time_cost_to_priority_ratio_exception = UserException(
             HTTPStatus.BAD_REQUEST,
             FovusApiValidator.__name__,
             'timeToCostPriorityRatio must be of the form "time/cost" where 0 <= time <= 1, '
             + "0 <= cost <= 1, and time + cost = 1",
         )
 
-        time, cost = time_cost_to_priority_ratio.split("/")
+        time, cost = self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_JOB_CONSTRAINTS][PAYLOAD_TIME_COST_PRIORITY_RATIO].split(
+            "/"
+        )
         time, cost = float(time), float(cost)
         for value in (time, cost):
             if value < 0 or value > 1:
                 raise time_cost_to_priority_ratio_exception
         if time + cost != 1:
             raise time_cost_to_priority_ratio_exception
 
-    @staticmethod
-    def _validate_parallelism_optimization_allowed_value(parallelism_optimization, scalable_parallelism):
-        if parallelism_optimization and not scalable_parallelism:
+    def _validate_parallelism_optimization_allowed_value(self):
+        if (
+            self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][PARALLELISM_OPTIMIZATION]
+            and not self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][SCALABLE_PARALLELISM]
+        ):
             raise UserException(
                 HTTPStatus.BAD_REQUEST,
                 FovusApiValidator.__name__,
                 "parallelismOptimization is only allowed to be set to true when scalableParallelism is set to true",
             )
 
-    @staticmethod
-    def _validate_min_max_vcpu(min_vcpu, max_vcpu):
-        if min_vcpu > max_vcpu:
+    def _validate_min_max_vcpu(self):
+        if (
+            self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MIN_VCPU]
+            > self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MAX_VCPU]
+        ):
             raise UserException(
                 HTTPStatus.BAD_REQUEST, FovusApiValidator.__name__, "minvCpu must be less than or equal to maxvCpu"
             )
 
-    @staticmethod
-    def _validate_min_max_gpu(min_gpu, max_gpu):
-        if min_gpu > max_gpu:
+    def _validate_min_max_gpu(self):
+        if (
+            self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MIN_GPU]
+            > self.payload[PAYLOAD_CONSTRAINTS][PAYLOAD_TASK_CONSTRAINTS][MAX_GPU]
+        ):
             raise UserException(
                 HTTPStatus.BAD_REQUEST, FovusApiValidator.__name__, "minGpu must be less than or equal to maxGpu"
             )
```

## Comparing `fovus-1.0.4.dist-info/LICENSE.txt` & `fovus-1.0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fovus-1.0.4.dist-info/METADATA` & `fovus-1.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fovus
-Version: 1.0.4
+Version: 1.0.5
 Summary: The Fovus Python CLI
 Author: Fovus Corporation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: boto3 (>=1.26.60)
 Requires-Dist: jsonschema (>=3.2.0)
@@ -78,15 +78,15 @@
 
 ### Password environment variable
 
 Export your Fovus password as an environment variable by following the instructions for your system:
 
 Unix-based systems
 ```
-export FOVUS_CLI_PASSWORD="your_password_here"
+export FOVUS_CLI_PASSWORD='your_password_here'
 ```
 
 Windows
 
 1. Run `setx FOVUS_CLI_PASSWORD "your_password_here"` in command prompt
 2. Close your command prompt and open a new one (to refresh the environment variables)
```

## Comparing `fovus-1.0.4.dist-info/RECORD` & `fovus-1.0.5.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 fovus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/root_config.py,sha256=onsSNaAhzMvRK8o82IkASh4EVkyMxVMPBlUXcUq1Lcg,65
 fovus/adapter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/adapter/aws_cognito_adapter.py,sha256=RsqnPW2spH2DKn6mDf4cgbd3KwICANS4uL7vt0zo6k8,3331
-fovus/adapter/fovus_api_adapter.py,sha256=GhvZWNSFcS3rqxgI6pavacnI_GbBO_kf1ZEaxmpVlRw,10856
+fovus/adapter/fovus_api_adapter.py,sha256=Y-NGC9vBM0gBJblxfYQfvqttacx7YOWATBT7YkcGkQM,19085
 fovus/adapter/fovus_s3_adapter.py,sha256=0O5IUT1WUk_i2GAoy_J3lZB0Onh4M2z6U-hX_lr1Lxs,8700
 fovus/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/cli/cli_action_runner.py,sha256=TYG2iJgfft0GgezuyyLtC_VxL0TmrV-HajeLuFSjVMo,13184
+fovus/cli/cli_action_runner.py,sha256=o2SHIqdEOvUkhlUY-ZtoHacCEt3LzrY4HFCOLNrtOU8,13450
 fovus/cli/documenter.py,sha256=uzpu25Wd8YXirM7oQPLG3hqgAZa2_H_YPz0i522qxyo,161
 fovus/cli/fovus_cli.py,sha256=6YyqZ6-gzmH2eXVlwwbg-jl4P_lRJn77qx1_cG_432U,475
-fovus/cli/fovus_cli_argument_parser.py,sha256=Uhm80S-6cml5lnALUl8J2IrnLM8-L0aBaodcsJRNALI,25901
+fovus/cli/fovus_cli_argument_parser.py,sha256=OgTmDTokaquT9qIcnMDy3Z5Aco7xaLuNDnv6ru85Z9g,25911
 fovus/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/config/config.py,sha256=LhikS-z0_0IL8uGJVDSf-HfPfq0a6_C3oOixw320sYM,138
 fovus/constants/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fovus/constants/benchmark_constants.py,sha256=liNu-qvuo6VFfwud2upeYakuk9fVvSOe60EX0KyCdx0,1278
 fovus/constants/cli_action_runner_constants.py,sha256=k_k3fQ1SgcMpm3Gm12Mhii4DVh3-AlHKeJMh5MreeMs,59
-fovus/constants/cli_constants.py,sha256=ZNH8qT5lbDw0haFB_qjQqkp8filVBQC7ZJtPvGz0YIE,8641
-fovus/constants/fovus_api_constants.py,sha256=IAWrzQwMbFVp7a7hmDp_wg3ETVIkvhd39bELbCxErlo,1446
+fovus/constants/cli_constants.py,sha256=1raw6jGzntHYdBEckvhU8gGuaNoOJ_jdLFYjZoVpRMY,8682
+fovus/constants/fovus_api_constants.py,sha256=so5TuaeO7r2ggQJwsUm1BReEtFxTI2lHlsna_92fcCI,2100
 fovus/constants/util_constants.py,sha256=tcIzvskdO_N9aYrNLLoqoASG76AVeiuexcfzG-IouPQ,194
 fovus/exception/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/exception/status_code_exception.py,sha256=HXfQ6E3gGSEg2dUxS6ccPN5kAgCC33nVzCuAy_zxN7o,291
 fovus/exception/system_exception.py,sha256=lzoDivDErUE47Cz3v9U1AhbzI4MQHTeYbvmn02myOHA,183
 fovus/exception/user_exception.py,sha256=Un3pq8s1a7gXdZ8MoHNhxE5xZz_fO4cBy4lE2n7uEzg,174
 fovus/fovus_provided_configs/FOVUS_example_job_config_containerized.json,sha256=FXKEiSlgg1-3NaDm5Sm0IuAJHyaTMV78yjwZ-PB651A,1054
 fovus/fovus_provided_configs/FOVUS_example_job_config_monolithic.json,sha256=S-wGqqE657jOq6ki83VeNcwefvIOtBnkZDgc5u-JGTk,1112
@@ -27,20 +28,20 @@
 fovus/fovus_provided_configs/FOVUS_user_config_template.json,sha256=HMCwX1ffMaUFonqxfv94c1ZlianfRTXal3BsYMxuRAE,42
 fovus/fovus_provided_configs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/schema/create_job_schema.json,sha256=rxVBkIytO6qvcLd_qmHtxkKJMvDb5SFFS33BUwOzSfQ,10183
 fovus/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fovus/util/aws_util.py,sha256=KX6DJIkwZ8ruToI8O0fK0TYEVxfyZI-p3NkRSSbGuVg,3389
 fovus/util/cli_action_runner_util.py,sha256=cPVVedOavu7nO_bbRS8wlipc2PCB-Q94BAMV3aopOYo,334
-fovus/util/file_util.py,sha256=DGC-DYXh4YUv1EJmpa2U_SVRqiW4na2DMRdEAIi9sic,4616
-fovus/util/fovus_api_util.py,sha256=7Auhoqjh0drGODn9U4zWG6e2eXlvCvRiuqQDpQCZz2A,2871
+fovus/util/file_util.py,sha256=S_sE2yzOrIEyDy6BjBW615lGWzTNx6yLhhGcaChxRis,4625
+fovus/util/fovus_api_util.py,sha256=1xb-lo8toBwZ1Pm5PHJ6POJ-LMsDvFFom64tqRNCfOQ,7357
 fovus/util/fovus_cli_argument_parser_util.py,sha256=kuVUIibYr_9crVH34aX-MotOwj_KBBt8R_bbbrEmiIw,1740
 fovus/util/fovus_s3_adapter_util.py,sha256=WQwqgaeVttAUTJ2MyO9KFXpaIsVFwzcUM3K6xZ5oeFU,1519
 fovus/util/util.py,sha256=i_mzAJDsIvvWEEOTVGYckYZInZe6EddwyJiiVQca7R4,533
 fovus/validator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fovus/validator/fovus_api_validator.py,sha256=2X108-S2IIJyxdX2PvN1mAhe1de-be09GRGeyDWfw5g,3935
-fovus-1.0.4.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
-fovus-1.0.4.dist-info/METADATA,sha256=FQcwbhgxsM32wCdsbv6MIXACjloN8DpCDSjOk9gX-to,8883
-fovus-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-fovus-1.0.4.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
-fovus-1.0.4.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
-fovus-1.0.4.dist-info/RECORD,,
+fovus/validator/fovus_api_validator.py,sha256=3_epp3QpaRmDColc2u0NwpAC9ud-EhivAKLM5EW8hNA,3732
+fovus-1.0.5.dist-info/LICENSE.txt,sha256=fchJSAB0_4gOri4wW-wCs_gpi7L_-ece0Cr4YBsWojc,14101
+fovus-1.0.5.dist-info/METADATA,sha256=Zug2BVdRkvAdGdaaxRQD_Bz0eNLFpCLCvIVHuqOL0F0,8883
+fovus-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+fovus-1.0.5.dist-info/entry_points.txt,sha256=TjKfUkIuYlXaVbtONHkk38PSJmraR93NMOef9drKHu0,51
+fovus-1.0.5.dist-info/top_level.txt,sha256=oMIzxBylwDA2FvFy-uGFm6CKP6EhsbVzUlpaUdwtYGw,6
+fovus-1.0.5.dist-info/RECORD,,
```

