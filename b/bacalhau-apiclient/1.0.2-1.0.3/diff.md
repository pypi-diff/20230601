# Comparing `tmp/bacalhau_apiclient-1.0.2.tar.gz` & `tmp/bacalhau_apiclient-1.0.3.tar.gz`

## Comparing `bacalhau_apiclient-1.0.2.tar` & `bacalhau_apiclient-1.0.3.tar`

### file list

```diff
@@ -1,183 +1,187 @@
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/.swagger-codegen-ignore
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/requirements.txt
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/setup.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/test-requirements.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/tox.ini
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/.swagger-codegen/VERSION
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/__init__.py
--rw-r--r--   0        0        0    25217 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api_client.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/configuration.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/rest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/__init__.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/default_api.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/health_api.py
--rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/job_api.py
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/misc_api.py
--rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/utils_api.py
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/__init__.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_execution_state_run_output.py
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_execution_state_state.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_create_payload_spec.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_spec.py
--rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_state_state.py
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_with_info_job.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_with_info_state.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_deal.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_docker.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_engine.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_network.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_publisher.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_resources.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofcancel_request_payload.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofevents_request_filters.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_oflog_request_payload.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofsubmit_request_payload.py
--rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/build_version_info.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/cancel_request.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/cancel_response.py
--rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/compute_node_info.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/deal.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/engine.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/event_filter_options.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/events_request.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/events_response.py
--rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/execution_state.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/execution_state_type.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/free_space.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/health_info.py
--rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_cancel_payload.py
--rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_create_payload.py
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_history.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_history_type.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_requester.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_spec_docker.py
--rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_spec_wasm.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_state.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_state_type.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_with_info.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/label_selector_requirement.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/list_request.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/list_response.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/log_request.py
--rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/logs_payload.py
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/metadata.py
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/mount_status.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/network.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/network_config.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/node_info.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/node_type.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/peer_addr_info.py
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/published_result.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/publisher.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/publisher_spec.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/resource_usage_config.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/resource_usage_data.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/results_response.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/run_command_result.py
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/s3_storage_spec.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/selection_operator.py
--rw-r--r--   0        0        0    14756 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/spec.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_change_execution_state_type.py
--rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_change_job_state_type.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_request.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_response.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/storage_source_type.py
--rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/storage_spec.py
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/submit_request.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/submit_response.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/verification_result.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/verifier.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/version_request.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/version_response.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfExecutionStateRunOutput.md
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfExecutionStateState.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobCreatePayloadSpec.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobSpec.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobSpecWasmEntryModule.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobStateState.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobWithInfoJob.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfJobWithInfoState.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfLabelSelectorRequirementOperator.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecDeal.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecDocker.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecEngine.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecNetwork.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecPublisher.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfSpecResources.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfStorageSpecStorageSource.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfcancelRequestPayload.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfeventsRequestFilters.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOflogRequestPayload.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/AllOfsubmitRequestPayload.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/BuildVersionInfo.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/CancelRequest.md
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/CancelResponse.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ComputeNodeInfo.md
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Deal.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/DefaultApi.md
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Engine.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/EventFilterOptions.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/EventsRequest.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/EventsResponse.md
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ExecutionState.md
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ExecutionStateType.md
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/FreeSpace.md
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/HealthApi.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/HealthInfo.md
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Job.md
--rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobApi.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobCancelPayload.md
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobCreatePayload.md
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobHistory.md
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobHistoryType.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobRequester.md
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobSpecDocker.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobSpecWasm.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobState.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobStateType.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/JobWithInfo.md
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/LabelSelectorRequirement.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ListRequest.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ListResponse.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/LogRequest.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/LogsPayload.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Metadata.md
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/MiscApi.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/MountStatus.md
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Network.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/NetworkConfig.md
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/NodeInfo.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/NodeType.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/PeerAddrInfo.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/PublishedResult.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Publisher.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/PublisherSpec.md
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ResourceUsageConfig.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ResourceUsageData.md
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/ResultsResponse.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/RunCommandResult.md
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/S3StorageSpec.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/SelectionOperator.md
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Spec.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StateChangeExecutionStateType.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StateChangeJobStateType.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StateRequest.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StateResponse.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StorageSourceType.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/StorageSpec.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/SubmitRequest.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/SubmitResponse.md
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/UtilsApi.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/VerificationResult.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/Verifier.md
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/VersionRequest.md
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/docs/VersionResponse.md
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/.gitignore
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/LICENSE
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9031 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/.swagger-codegen-ignore
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/requirements.txt
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/test-requirements.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/tox.ini
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/__init__.py
+-rw-r--r--   0        0        0    25217 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api_client.py
+-rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/configuration.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/rest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/__init__.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/default_api.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/health_api.py
+-rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/job_api.py
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/misc_api.py
+-rw-r--r--   0        0        0    24993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/utils_api.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/__init__.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_execution_state_run_output.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_execution_state_state.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_create_payload_spec.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_spec.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_spec_language_job_context.py
+-rw-r--r--   0        0        0     2993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_state_state.py
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_with_info_job.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_with_info_state.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_deal.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_docker.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_engine.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_network.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_publisher.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_resources.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofcancel_request_payload.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofevents_request_filters.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_oflog_request_payload.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofsubmit_request_payload.py
+-rw-r--r--   0        0        0     7138 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/build_version_info.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/cancel_request.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/cancel_response.py
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/compute_node_info.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/deal.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/engine.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/event_filter_options.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/events_request.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/events_response.py
+-rw-r--r--   0        0        0    14210 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/execution_state.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/execution_state_type.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/free_space.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/health_info.py
+-rw-r--r--   0        0        0     4525 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_cancel_payload.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_create_payload.py
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_history.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_history_type.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_requester.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_spec_docker.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_spec_language.py
+-rw-r--r--   0        0        0     7781 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_spec_wasm.py
+-rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_state.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_state_type.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_with_info.py
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/label_selector_requirement.py
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/list_request.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/list_response.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/log_request.py
+-rw-r--r--   0        0        0     6848 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/logs_payload.py
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/metadata.py
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/mount_status.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/network.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/network_config.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/node_info.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/node_type.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/peer_addr_info.py
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/published_result.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/publisher.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/publisher_spec.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/resource_usage_config.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/resource_usage_data.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/results_response.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/run_command_result.py
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/s3_storage_spec.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/selection_operator.py
+-rw-r--r--   0        0        0    15417 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/spec.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_change_execution_state_type.py
+-rw-r--r--   0        0        0     3971 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_change_job_state_type.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_request.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_response.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/storage_source_type.py
+-rw-r--r--   0        0        0    11084 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/storage_spec.py
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/submit_request.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/submit_response.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/verification_result.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/verifier.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/version_request.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/version_response.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfExecutionStateRunOutput.md
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfExecutionStateState.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobCreatePayloadSpec.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobSpec.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobSpecLanguageJobContext.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobSpecWasmEntryModule.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobStateState.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobWithInfoJob.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfJobWithInfoState.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfLabelSelectorRequirementOperator.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecDeal.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecDocker.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecEngine.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecNetwork.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecPublisher.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfSpecResources.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfStorageSpecStorageSource.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfcancelRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfeventsRequestFilters.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOflogRequestPayload.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/AllOfsubmitRequestPayload.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/BuildVersionInfo.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/CancelRequest.md
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/CancelResponse.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ComputeNodeInfo.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Deal.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/DefaultApi.md
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Engine.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/EventFilterOptions.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/EventsRequest.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/EventsResponse.md
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ExecutionState.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ExecutionStateType.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/FreeSpace.md
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/HealthApi.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/HealthInfo.md
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Job.md
+-rw-r--r--   0        0        0    13414 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobApi.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobCancelPayload.md
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobCreatePayload.md
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobHistory.md
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobHistoryType.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobRequester.md
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobSpecDocker.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobSpecLanguage.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobSpecWasm.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobState.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobStateType.md
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/JobWithInfo.md
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/LabelSelectorRequirement.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ListRequest.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ListResponse.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/LogRequest.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/LogsPayload.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Metadata.md
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/MiscApi.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/MountStatus.md
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Network.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/NetworkConfig.md
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/NodeInfo.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/NodeType.md
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/PeerAddrInfo.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/PublishedResult.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Publisher.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/PublisherSpec.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ResourceUsageConfig.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ResourceUsageData.md
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/ResultsResponse.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/RunCommandResult.md
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/S3StorageSpec.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/SelectionOperator.md
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Spec.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StateChangeExecutionStateType.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StateChangeJobStateType.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StateRequest.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StateResponse.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StorageSourceType.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/StorageSpec.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/SubmitRequest.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/SubmitResponse.md
+-rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/UtilsApi.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/VerificationResult.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/Verifier.md
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/VersionRequest.md
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/docs/VersionResponse.md
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/.gitignore
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 bacalhau_apiclient-1.0.3/PKG-INFO
```

### Comparing `bacalhau_apiclient-1.0.2/.swagger-codegen-ignore` & `bacalhau_apiclient-1.0.3/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/setup.py` & `bacalhau_apiclient-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: team@bacalhau.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "bacalhau_apiclient"
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/__init__.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from bacalhau_apiclient.api_client import ApiClient
 from bacalhau_apiclient.configuration import Configuration
 # import models into sdk package
 from bacalhau_apiclient.models.all_of_execution_state_run_output import AllOfExecutionStateRunOutput
 from bacalhau_apiclient.models.all_of_execution_state_state import AllOfExecutionStateState
 from bacalhau_apiclient.models.all_of_job_create_payload_spec import AllOfJobCreatePayloadSpec
 from bacalhau_apiclient.models.all_of_job_spec import AllOfJobSpec
+from bacalhau_apiclient.models.all_of_job_spec_language_job_context import AllOfJobSpecLanguageJobContext
 from bacalhau_apiclient.models.all_of_job_spec_wasm_entry_module import AllOfJobSpecWasmEntryModule
 from bacalhau_apiclient.models.all_of_job_state_state import AllOfJobStateState
 from bacalhau_apiclient.models.all_of_job_with_info_job import AllOfJobWithInfoJob
 from bacalhau_apiclient.models.all_of_job_with_info_state import AllOfJobWithInfoState
 from bacalhau_apiclient.models.all_of_label_selector_requirement_operator import AllOfLabelSelectorRequirementOperator
 from bacalhau_apiclient.models.all_of_spec_deal import AllOfSpecDeal
 from bacalhau_apiclient.models.all_of_spec_docker import AllOfSpecDocker
@@ -60,14 +61,15 @@
 from bacalhau_apiclient.models.job import Job
 from bacalhau_apiclient.models.job_cancel_payload import JobCancelPayload
 from bacalhau_apiclient.models.job_create_payload import JobCreatePayload
 from bacalhau_apiclient.models.job_history import JobHistory
 from bacalhau_apiclient.models.job_history_type import JobHistoryType
 from bacalhau_apiclient.models.job_requester import JobRequester
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
+from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_wasm import JobSpecWasm
 from bacalhau_apiclient.models.job_state import JobState
 from bacalhau_apiclient.models.job_state_type import JobStateType
 from bacalhau_apiclient.models.job_with_info import JobWithInfo
 from bacalhau_apiclient.models.label_selector_requirement import LabelSelectorRequirement
 from bacalhau_apiclient.models.list_request import ListRequest
 from bacalhau_apiclient.models.list_response import ListResponse
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api_client.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.2/python'
+        self.user_agent = 'Swagger-Codegen/1.0.3/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/configuration.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,9 +236,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: ${PYPI_VERSION}\n"\
-               "SDK Package Version: 1.0.2".\
+               "SDK Package Version: 1.0.3".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/rest.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/rest.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/default_api.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/default_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/health_api.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/health_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/job_api.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/job_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/misc_api.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/misc_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/api/utils_api.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/api/utils_api.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/__init__.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from __future__ import absolute_import
 
 # import models into model package
 from bacalhau_apiclient.models.all_of_execution_state_run_output import AllOfExecutionStateRunOutput
 from bacalhau_apiclient.models.all_of_execution_state_state import AllOfExecutionStateState
 from bacalhau_apiclient.models.all_of_job_create_payload_spec import AllOfJobCreatePayloadSpec
 from bacalhau_apiclient.models.all_of_job_spec import AllOfJobSpec
+from bacalhau_apiclient.models.all_of_job_spec_language_job_context import AllOfJobSpecLanguageJobContext
 from bacalhau_apiclient.models.all_of_job_spec_wasm_entry_module import AllOfJobSpecWasmEntryModule
 from bacalhau_apiclient.models.all_of_job_state_state import AllOfJobStateState
 from bacalhau_apiclient.models.all_of_job_with_info_job import AllOfJobWithInfoJob
 from bacalhau_apiclient.models.all_of_job_with_info_state import AllOfJobWithInfoState
 from bacalhau_apiclient.models.all_of_label_selector_requirement_operator import AllOfLabelSelectorRequirementOperator
 from bacalhau_apiclient.models.all_of_spec_deal import AllOfSpecDeal
 from bacalhau_apiclient.models.all_of_spec_docker import AllOfSpecDocker
@@ -50,14 +51,15 @@
 from bacalhau_apiclient.models.job import Job
 from bacalhau_apiclient.models.job_cancel_payload import JobCancelPayload
 from bacalhau_apiclient.models.job_create_payload import JobCreatePayload
 from bacalhau_apiclient.models.job_history import JobHistory
 from bacalhau_apiclient.models.job_history_type import JobHistoryType
 from bacalhau_apiclient.models.job_requester import JobRequester
 from bacalhau_apiclient.models.job_spec_docker import JobSpecDocker
+from bacalhau_apiclient.models.job_spec_language import JobSpecLanguage
 from bacalhau_apiclient.models.job_spec_wasm import JobSpecWasm
 from bacalhau_apiclient.models.job_state import JobState
 from bacalhau_apiclient.models.job_state_type import JobStateType
 from bacalhau_apiclient.models.job_with_info import JobWithInfo
 from bacalhau_apiclient.models.label_selector_requirement import LabelSelectorRequirement
 from bacalhau_apiclient.models.list_request import ListRequest
 from bacalhau_apiclient.models.list_response import ListResponse
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_execution_state_run_output.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_execution_state_run_output.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_execution_state_state.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_execution_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_create_payload_spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_create_payload_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_spec_wasm_entry_module.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_state_state.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_state_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_with_info_job.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_with_info_job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_job_with_info_state.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_job_with_info_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_label_selector_requirement_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_deal.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_docker.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_engine.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_engine.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_network.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_publisher.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_publisher.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_spec_resources.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_spec_resources.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_of_storage_spec_storage_source.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofcancel_request_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofcancel_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofevents_request_filters.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofevents_request_filters.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_oflog_request_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_oflog_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/all_ofsubmit_request_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/all_ofsubmit_request_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/build_version_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/build_version_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/cancel_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/cancel_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/cancel_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/cancel_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/compute_node_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/compute_node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/deal.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/deal.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/engine.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     allowed enum values
     """
     _0 = "0"
     _1 = "1"
     _2 = "2"
     _3 = "3"
     _4 = "4"
+    _5 = "5"
+    _6 = "6"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/event_filter_options.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/event_filter_options.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/events_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/events_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/events_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/events_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/execution_state.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/execution_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/execution_state_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/free_space.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/free_space.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/health_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/health_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_cancel_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_cancel_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_create_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_create_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_history.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_history.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_history_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_history_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_requester.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_requester.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_spec_docker.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_spec_docker.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_spec_wasm.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_spec_wasm.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_state.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_state.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_state_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/job_with_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/job_with_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/label_selector_requirement.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/label_selector_requirement.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/list_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/list_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/list_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/list_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/log_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/log_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/logs_payload.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/logs_payload.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/metadata.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/metadata.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/mount_status.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/mount_status.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/network.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/network.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/network_config.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/network_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/node_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/node_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/node_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/node_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/peer_addr_info.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/peer_addr_info.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/published_result.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/published_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/publisher.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/publisher.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/publisher_spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/publisher_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/resource_usage_config.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/resource_usage_config.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/resource_usage_data.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/resource_usage_data.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/results_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/results_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/run_command_result.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/run_command_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/s3_storage_spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/s3_storage_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/selection_operator.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/selection_operator.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     """
     swagger_types = {
         'annotations': 'list[str]',
         'deal': 'AllOfSpecDeal',
         'do_not_track': 'bool',
         'docker': 'AllOfSpecDocker',
         'engine': 'AllOfSpecEngine',
+        'language': 'JobSpecLanguage',
         'network': 'AllOfSpecNetwork',
         'node_selectors': 'list[LabelSelectorRequirement]',
         'publisher': 'AllOfSpecPublisher',
         'publisher_spec': 'PublisherSpec',
         'resources': 'AllOfSpecResources',
         'timeout': 'float',
         'verifier': 'Verifier',
@@ -47,33 +48,35 @@
 
     attribute_map = {
         'annotations': 'Annotations',
         'deal': 'Deal',
         'do_not_track': 'DoNotTrack',
         'docker': 'Docker',
         'engine': 'Engine',
+        'language': 'Language',
         'network': 'Network',
         'node_selectors': 'NodeSelectors',
         'publisher': 'Publisher',
         'publisher_spec': 'PublisherSpec',
         'resources': 'Resources',
         'timeout': 'Timeout',
         'verifier': 'Verifier',
         'wasm': 'Wasm',
         'inputs': 'inputs',
         'outputs': 'outputs'
     }
 
-    def __init__(self, annotations=None, deal=None, do_not_track=None, docker=None, engine=None, network=None, node_selectors=None, publisher=None, publisher_spec=None, resources=None, timeout=None, verifier=None, wasm=None, inputs=None, outputs=None):  # noqa: E501
+    def __init__(self, annotations=None, deal=None, do_not_track=None, docker=None, engine=None, language=None, network=None, node_selectors=None, publisher=None, publisher_spec=None, resources=None, timeout=None, verifier=None, wasm=None, inputs=None, outputs=None):  # noqa: E501
         """Spec - a model defined in Swagger"""  # noqa: E501
         self._annotations = None
         self._deal = None
         self._do_not_track = None
         self._docker = None
         self._engine = None
+        self._language = None
         self._network = None
         self._node_selectors = None
         self._publisher = None
         self._publisher_spec = None
         self._resources = None
         self._timeout = None
         self._verifier = None
@@ -87,14 +90,16 @@
             self.deal = deal
         if do_not_track is not None:
             self.do_not_track = do_not_track
         if docker is not None:
             self.docker = docker
         if engine is not None:
             self.engine = engine
+        if language is not None:
+            self.language = language
         if network is not None:
             self.network = network
         if node_selectors is not None:
             self.node_selectors = node_selectors
         if publisher is not None:
             self.publisher = publisher
         if publisher_spec is not None:
@@ -224,14 +229,35 @@
         :param engine: The engine of this Spec.  # noqa: E501
         :type: AllOfSpecEngine
         """
 
         self._engine = engine
 
     @property
+    def language(self):
+        """Gets the language of this Spec.  # noqa: E501
+
+
+        :return: The language of this Spec.  # noqa: E501
+        :rtype: JobSpecLanguage
+        """
+        return self._language
+
+    @language.setter
+    def language(self, language):
+        """Sets the language of this Spec.
+
+
+        :param language: The language of this Spec.  # noqa: E501
+        :type: JobSpecLanguage
+        """
+
+        self._language = language
+
+    @property
     def network(self):
         """Gets the network of this Spec.  # noqa: E501
 
         The type of networking access that the job needs  # noqa: E501
 
         :return: The network of this Spec.  # noqa: E501
         :rtype: AllOfSpecNetwork
```

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_change_execution_state_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_change_execution_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_change_job_state_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_change_job_state_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/state_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/state_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/storage_source_type.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/storage_source_type.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/storage_spec.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/storage_spec.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/submit_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/submit_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/submit_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/submit_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/verification_result.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/verifier.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/verifier.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/version_request.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/version_request.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/bacalhau_apiclient/models/version_response.py` & `bacalhau_apiclient-1.0.3/bacalhau_apiclient/models/version_response.py`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/BuildVersionInfo.md` & `bacalhau_apiclient-1.0.3/docs/BuildVersionInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/CancelRequest.md` & `bacalhau_apiclient-1.0.3/docs/CancelRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/ComputeNodeInfo.md` & `bacalhau_apiclient-1.0.3/docs/ComputeNodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/Deal.md` & `bacalhau_apiclient-1.0.3/docs/Deal.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/DefaultApi.md` & `bacalhau_apiclient-1.0.3/docs/DefaultApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/ExecutionState.md` & `bacalhau_apiclient-1.0.3/docs/ExecutionState.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/HealthApi.md` & `bacalhau_apiclient-1.0.3/docs/HealthApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobApi.md` & `bacalhau_apiclient-1.0.3/docs/JobApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobCancelPayload.md` & `bacalhau_apiclient-1.0.3/docs/JobCancelPayload.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobHistory.md` & `bacalhau_apiclient-1.0.3/docs/JobHistory.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobRequester.md` & `bacalhau_apiclient-1.0.3/docs/JobRequester.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobSpecDocker.md` & `bacalhau_apiclient-1.0.3/docs/JobSpecDocker.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobSpecWasm.md` & `bacalhau_apiclient-1.0.3/docs/JobSpecWasm.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobState.md` & `bacalhau_apiclient-1.0.3/docs/JobState.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/JobWithInfo.md` & `bacalhau_apiclient-1.0.3/docs/JobWithInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/LabelSelectorRequirement.md` & `bacalhau_apiclient-1.0.3/docs/LabelSelectorRequirement.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/ListRequest.md` & `bacalhau_apiclient-1.0.3/docs/ListRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/LogRequest.md` & `bacalhau_apiclient-1.0.3/docs/LogRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/LogsPayload.md` & `bacalhau_apiclient-1.0.3/docs/LogsPayload.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/Metadata.md` & `bacalhau_apiclient-1.0.3/docs/Metadata.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/MiscApi.md` & `bacalhau_apiclient-1.0.3/docs/MiscApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/NodeInfo.md` & `bacalhau_apiclient-1.0.3/docs/NodeInfo.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/ResourceUsageConfig.md` & `bacalhau_apiclient-1.0.3/docs/ResourceUsageConfig.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/RunCommandResult.md` & `bacalhau_apiclient-1.0.3/docs/RunCommandResult.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/S3StorageSpec.md` & `bacalhau_apiclient-1.0.3/docs/S3StorageSpec.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/Spec.md` & `bacalhau_apiclient-1.0.3/docs/Spec.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **annotations** | **list[str]** | Annotations on the job - could be user or machine assigned | [optional] 
 **deal** | **AllOfSpecDeal** | The deal the client has made, such as which job bids they have accepted. | [optional] 
 **do_not_track** | **bool** | Do not track specified by the client | [optional] 
 **docker** | **AllOfSpecDocker** | executor specific data | [optional] 
 **engine** | **AllOfSpecEngine** | e.g. docker or language | [optional] 
+**language** | [**JobSpecLanguage**](JobSpecLanguage.md) |  | [optional] 
 **network** | **AllOfSpecNetwork** | The type of networking access that the job needs | [optional] 
 **node_selectors** | [**list[LabelSelectorRequirement]**](LabelSelectorRequirement.md) | NodeSelectors is a selector which must be true for the compute node to run this job. | [optional] 
 **publisher** | **AllOfSpecPublisher** | there can be multiple publishers for the job deprecated: use PublisherSpec instead | [optional] 
 **publisher_spec** | [**PublisherSpec**](PublisherSpec.md) |  | [optional] 
 **resources** | **AllOfSpecResources** | the compute (cpu, ram) resources this job requires | [optional] 
 **timeout** | **float** | How long a job can run in seconds before it is killed. This includes the time required to run, verify and publish results | [optional] 
 **verifier** | [**Verifier**](Verifier.md) |  | [optional]
```

### Comparing `bacalhau_apiclient-1.0.2/docs/StorageSpec.md` & `bacalhau_apiclient-1.0.3/docs/StorageSpec.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/SubmitRequest.md` & `bacalhau_apiclient-1.0.3/docs/SubmitRequest.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/docs/UtilsApi.md` & `bacalhau_apiclient-1.0.3/docs/UtilsApi.md`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/.gitignore` & `bacalhau_apiclient-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/LICENSE` & `bacalhau_apiclient-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bacalhau_apiclient-1.0.2/README.md` & `bacalhau_apiclient-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 1.0.2
+- Package version: 1.0.3
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
 
@@ -101,14 +101,15 @@
 
 ## Documentation For Models
 
  - [AllOfExecutionStateRunOutput](docs/AllOfExecutionStateRunOutput.md)
  - [AllOfExecutionStateState](docs/AllOfExecutionStateState.md)
  - [AllOfJobCreatePayloadSpec](docs/AllOfJobCreatePayloadSpec.md)
  - [AllOfJobSpec](docs/AllOfJobSpec.md)
+ - [AllOfJobSpecLanguageJobContext](docs/AllOfJobSpecLanguageJobContext.md)
  - [AllOfJobSpecWasmEntryModule](docs/AllOfJobSpecWasmEntryModule.md)
  - [AllOfJobStateState](docs/AllOfJobStateState.md)
  - [AllOfJobWithInfoJob](docs/AllOfJobWithInfoJob.md)
  - [AllOfJobWithInfoState](docs/AllOfJobWithInfoState.md)
  - [AllOfLabelSelectorRequirementOperator](docs/AllOfLabelSelectorRequirementOperator.md)
  - [AllOfSpecDeal](docs/AllOfSpecDeal.md)
  - [AllOfSpecDocker](docs/AllOfSpecDocker.md)
@@ -137,14 +138,15 @@
  - [Job](docs/Job.md)
  - [JobCancelPayload](docs/JobCancelPayload.md)
  - [JobCreatePayload](docs/JobCreatePayload.md)
  - [JobHistory](docs/JobHistory.md)
  - [JobHistoryType](docs/JobHistoryType.md)
  - [JobRequester](docs/JobRequester.md)
  - [JobSpecDocker](docs/JobSpecDocker.md)
+ - [JobSpecLanguage](docs/JobSpecLanguage.md)
  - [JobSpecWasm](docs/JobSpecWasm.md)
  - [JobState](docs/JobState.md)
  - [JobStateType](docs/JobStateType.md)
  - [JobWithInfo](docs/JobWithInfo.md)
  - [LabelSelectorRequirement](docs/LabelSelectorRequirement.md)
  - [ListRequest](docs/ListRequest.md)
  - [ListResponse](docs/ListResponse.md)
```

### Comparing `bacalhau_apiclient-1.0.2/pyproject.toml` & `bacalhau_apiclient-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bacalhau_apiclient"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
 { name="Enrico Rotundo", email="enrico.rotundo@gmail.com" },
 ]
 description = "A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python"
 readme = "README.md"
 requires-python = ">=3.6.2"
 classifiers = [
```

### Comparing `bacalhau_apiclient-1.0.2/PKG-INFO` & `bacalhau_apiclient-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacalhau_apiclient
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python client for the Bacalhau public API - https://github.com/bacalhau-project/bacalhau/tree/main/clients/python
 Project-URL: Homepage, https://github.com/bacalhau-project/bacalhau/
 Project-URL: Bug Tracker, https://github.com/bacalhau-project/bacalhau/issues
 Author-email: Enrico Rotundo <enrico.rotundo@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 
 # bacalhau_apiclient
 This page is the reference of the Bacalhau REST API. Project docs are available at https://docs.bacalhau.org/. Find more information about Bacalhau at https://github.com/bacalhau-project/bacalhau.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: ${PYPI_VERSION}
-- Package version: 1.0.2
+- Package version: 1.0.3
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 For more information, please visit [https://github.com/bacalhau-project/bacalhau](https://github.com/bacalhau-project/bacalhau)
 
 ## Requirements.
 
 Python 3.6+
 
@@ -114,14 +114,15 @@
 
 ## Documentation For Models
 
  - [AllOfExecutionStateRunOutput](docs/AllOfExecutionStateRunOutput.md)
  - [AllOfExecutionStateState](docs/AllOfExecutionStateState.md)
  - [AllOfJobCreatePayloadSpec](docs/AllOfJobCreatePayloadSpec.md)
  - [AllOfJobSpec](docs/AllOfJobSpec.md)
+ - [AllOfJobSpecLanguageJobContext](docs/AllOfJobSpecLanguageJobContext.md)
  - [AllOfJobSpecWasmEntryModule](docs/AllOfJobSpecWasmEntryModule.md)
  - [AllOfJobStateState](docs/AllOfJobStateState.md)
  - [AllOfJobWithInfoJob](docs/AllOfJobWithInfoJob.md)
  - [AllOfJobWithInfoState](docs/AllOfJobWithInfoState.md)
  - [AllOfLabelSelectorRequirementOperator](docs/AllOfLabelSelectorRequirementOperator.md)
  - [AllOfSpecDeal](docs/AllOfSpecDeal.md)
  - [AllOfSpecDocker](docs/AllOfSpecDocker.md)
@@ -150,14 +151,15 @@
  - [Job](docs/Job.md)
  - [JobCancelPayload](docs/JobCancelPayload.md)
  - [JobCreatePayload](docs/JobCreatePayload.md)
  - [JobHistory](docs/JobHistory.md)
  - [JobHistoryType](docs/JobHistoryType.md)
  - [JobRequester](docs/JobRequester.md)
  - [JobSpecDocker](docs/JobSpecDocker.md)
+ - [JobSpecLanguage](docs/JobSpecLanguage.md)
  - [JobSpecWasm](docs/JobSpecWasm.md)
  - [JobState](docs/JobState.md)
  - [JobStateType](docs/JobStateType.md)
  - [JobWithInfo](docs/JobWithInfo.md)
  - [LabelSelectorRequirement](docs/LabelSelectorRequirement.md)
  - [ListRequest](docs/ListRequest.md)
  - [ListResponse](docs/ListResponse.md)
```

