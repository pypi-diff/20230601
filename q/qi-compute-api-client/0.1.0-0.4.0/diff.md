# Comparing `tmp/qi_compute_api_client-0.1.0.tar.gz` & `tmp/qi_compute_api_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qi_compute_api_client-0.1.0.tar", max compression
+gzip compressed data, was "qi_compute_api_client-0.4.0.tar", max compression
```

## Comparing `qi_compute_api_client-0.1.0.tar` & `qi_compute_api_client-0.4.0.tar`

### file list

```diff
@@ -1,136 +1,137 @@
--rw-r--r--   0        0        0    11357 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/LICENSE.md
--rw-r--r--   0        0        0    15617 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/README.md
--rw-r--r--   0        0        0     4600 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/__init__.py
--rw-r--r--   0        0        0     1182 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/__init__.py
--rw-r--r--   0        0        0    31237 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/algorithms_api.py
--rw-r--r--   0        0        0    36454 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/batch_runs_api.py
--rw-r--r--   0        0        0    23963 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/commits_api.py
--rw-r--r--   0        0        0    23759 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/files_api.py
--rw-r--r--   0        0        0    19534 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/final_results_api.py
--rw-r--r--   0        0        0    12331 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/languages_api.py
--rw-r--r--   0        0        0    23961 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/members_api.py
--rw-r--r--   0        0        0    19369 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/metadata_api.py
--rw-r--r--   0        0        0    23668 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/permissions_api.py
--rw-r--r--   0        0        0    38011 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/projects_api.py
--rw-r--r--   0        0        0    24760 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/reservations_api.py
--rw-r--r--   0        0        0    19077 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/results_api.py
--rw-r--r--   0        0        0    29515 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/runs_api.py
--rw-r--r--   0        0        0    12013 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/runtime_api.py
--rw-r--r--   0        0        0    12223 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/runtime_types_api.py
--rw-r--r--   0        0        0    11888 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/teams_api.py
--rw-r--r--   0        0        0    12189 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/transactions_api.py
--rw-r--r--   0        0        0    23759 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api/users_api.py
--rw-r--r--   0        0        0    27838 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/api_client.py
--rw-r--r--   0        0        0    15871 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/configuration.py
--rw-r--r--   0        0        0      591 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/Algorithm.md
--rw-r--r--   0        0        0      570 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/AlgorithmIn.md
--rw-r--r--   0        0        0      308 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/AlgorithmType.md
--rw-r--r--   0        0        0     9718 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/AlgorithmsApi.md
--rw-r--r--   0        0        0      900 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/BatchRun.md
--rw-r--r--   0        0        0      353 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/BatchRunIn.md
--rw-r--r--   0        0        0      309 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/BatchRunStatus.md
--rw-r--r--   0        0        0    11613 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/BatchRunsApi.md
--rw-r--r--   0        0        0      445 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/Commit.md
--rw-r--r--   0        0        0      377 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/CommitIn.md
--rw-r--r--   0        0        0     7358 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/CommitsApi.md
--rw-r--r--   0        0        0      307 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/CompileStage.md
--rw-r--r--   0        0        0      301 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/Domain.md
--rw-r--r--   0        0        0      678 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/File.md
--rw-r--r--   0        0        0      668 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/FileIn.md
--rw-r--r--   0        0        0     7159 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/FilesApi.md
--rw-r--r--   0        0        0      434 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/FinalResult.md
--rw-r--r--   0        0        0      366 2023-01-13 22:55:39.140416 qi_compute_api_client-0.1.0/compute_api_client/docs/FinalResultIn.md
--rw-r--r--   0        0        0     6301 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/FinalResultsApi.md
--rw-r--r--   0        0        0      323 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/HTTPNotFoundError.md
--rw-r--r--   0        0        0      376 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/HTTPValidationError.md
--rw-r--r--   0        0        0      363 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Language.md
--rw-r--r--   0        0        0     3913 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/LanguagesApi.md
--rw-r--r--   0        0        0      292 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/LocationInner.md
--rw-r--r--   0        0        0      498 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Member.md
--rw-r--r--   0        0        0      477 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/MemberIn.md
--rw-r--r--   0        0        0     7355 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/MembersApi.md
--rw-r--r--   0        0        0      427 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Metadata.md
--rw-r--r--   0        0        0     6104 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/MetadataApi.md
--rw-r--r--   0        0        0      359 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/MetadataIn.md
--rw-r--r--   0        0        0      368 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Permission.md
--rw-r--r--   0        0        0      342 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/PermissionGroup.md
--rw-r--r--   0        0        0     7761 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/PermissionsApi.md
--rw-r--r--   0        0        0      500 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Project.md
--rw-r--r--   0        0        0      432 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ProjectIn.md
--rw-r--r--   0        0        0      468 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ProjectPatch.md
--rw-r--r--   0        0        0    11589 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ProjectsApi.md
--rw-r--r--   0        0        0      555 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Reservation.md
--rw-r--r--   0        0        0      428 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ReservationIn.md
--rw-r--r--   0        0        0     8002 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ReservationsApi.md
--rw-r--r--   0        0        0      770 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Result.md
--rw-r--r--   0        0        0      702 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ResultIn.md
--rw-r--r--   0        0        0     5868 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ResultsApi.md
--rw-r--r--   0        0        0      299 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Role.md
--rw-r--r--   0        0        0      792 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Run.md
--rw-r--r--   0        0        0      535 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RunIn.md
--rw-r--r--   0        0        0      304 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RunStatus.md
--rw-r--r--   0        0        0     8879 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RunsApi.md
--rw-r--r--   0        0        0      639 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Runtime.md
--rw-r--r--   0        0        0     3694 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeApi.md
--rw-r--r--   0        0        0      308 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeStatus.md
--rw-r--r--   0        0        0      617 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeType.md
--rw-r--r--   0        0        0     3924 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeTypesApi.md
--rw-r--r--   0        0        0      304 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ShareType.md
--rw-r--r--   0        0        0      422 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Team.md
--rw-r--r--   0        0        0     3564 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/TeamsApi.md
--rw-r--r--   0        0        0      609 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/Transaction.md
--rw-r--r--   0        0        0     3893 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/TransactionsApi.md
--rw-r--r--   0        0        0      607 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/User.md
--rw-r--r--   0        0        0      586 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/UserIn.md
--rw-r--r--   0        0        0     7159 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/UsersApi.md
--rw-r--r--   0        0        0      403 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/docs/ValidationError.md
--rw-r--r--   0        0        0     5143 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/exceptions.py
--rw-r--r--   0        0        0     2981 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/__init__.py
--rw-r--r--   0        0        0     8684 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/algorithm.py
--rw-r--r--   0        0        0     7545 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/algorithm_in.py
--rw-r--r--   0        0        0     3195 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/algorithm_type.py
--rw-r--r--   0        0        0    14456 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/batch_run.py
--rw-r--r--   0        0        0     5910 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/batch_run_in.py
--rw-r--r--   0        0        0     3304 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/batch_run_status.py
--rw-r--r--   0        0        0     8312 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/commit.py
--rw-r--r--   0        0        0     6318 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/commit_in.py
--rw-r--r--   0        0        0     3275 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/compile_stage.py
--rw-r--r--   0        0        0     3215 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/domain.py
--rw-r--r--   0        0        0    10593 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/file.py
--rw-r--r--   0        0        0     9327 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/file_in.py
--rw-r--r--   0        0        0     7123 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/final_result.py
--rw-r--r--   0        0        0     5081 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/final_result_in.py
--rw-r--r--   0        0        0     3868 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/http_not_found_error.py
--rw-r--r--   0        0        0     3782 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/http_validation_error.py
--rw-r--r--   0        0        0     6196 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/language.py
--rw-r--r--   0        0        0     3052 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/location_inner.py
--rw-r--r--   0        0        0     8530 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/member.py
--rw-r--r--   0        0        0     7403 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/member_in.py
--rw-r--r--   0        0        0     7015 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/metadata.py
--rw-r--r--   0        0        0     4997 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/metadata_in.py
--rw-r--r--   0        0        0     6303 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/permission.py
--rw-r--r--   0        0        0     5248 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/permission_group.py
--rw-r--r--   0        0        0     8855 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/project.py
--rw-r--r--   0        0        0     6861 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/project_in.py
--rw-r--r--   0        0        0     6448 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/project_patch.py
--rw-r--r--   0        0        0    10862 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/reservation.py
--rw-r--r--   0        0        0     7732 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/reservation_in.py
--rw-r--r--   0        0        0    14897 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/result.py
--rw-r--r--   0        0        0    12959 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/result_in.py
--rw-r--r--   0        0        0     3153 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/role.py
--rw-r--r--   0        0        0    11632 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/run.py
--rw-r--r--   0        0        0     6879 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/run_in.py
--rw-r--r--   0        0        0     3290 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/run_status.py
--rw-r--r--   0        0        0    11268 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/runtime.py
--rw-r--r--   0        0        0     3273 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/runtime_status.py
--rw-r--r--   0        0        0    11585 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/runtime_type.py
--rw-r--r--   0        0        0     3212 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/share_type.py
--rw-r--r--   0        0        0     6842 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/team.py
--rw-r--r--   0        0        0    10913 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/transaction.py
--rw-r--r--   0        0        0     8950 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/user.py
--rw-r--r--   0        0        0     7847 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/user_in.py
--rw-r--r--   0        0        0     5308 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/models/validation_error.py
--rw-r--r--   0        0        0     9931 2023-01-13 22:55:39.144416 qi_compute_api_client-0.1.0/compute_api_client/rest.py
--rw-r--r--   0        0        0     1170 2023-01-13 22:55:49.912438 qi_compute_api_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    16688 1970-01-01 00:00:00.000000 qi_compute_api_client-0.1.0/setup.py
--rw-r--r--   0        0        0    16882 1970-01-01 00:00:00.000000 qi_compute_api_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0    16473 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/README.md
+-rw-r--r--   0        0        0     4692 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/__init__.py
+-rw-r--r--   0        0        0    31278 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/algorithms_api.py
+-rw-r--r--   0        0        0    36523 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/batch_runs_api.py
+-rw-r--r--   0        0        0    23998 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/commits_api.py
+-rw-r--r--   0        0        0    23794 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/files_api.py
+-rw-r--r--   0        0        0    19563 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/final_results_api.py
+-rw-r--r--   0        0        0    12343 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/languages_api.py
+-rw-r--r--   0        0        0    23985 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/members_api.py
+-rw-r--r--   0        0        0    19387 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/metadata_api.py
+-rw-r--r--   0        0        0    23692 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/permissions_api.py
+-rw-r--r--   0        0        0    38047 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/projects_api.py
+-rw-r--r--   0        0        0    24784 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/reservations_api.py
+-rw-r--r--   0        0        0    19106 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/results_api.py
+-rw-r--r--   0        0        0    29556 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runs_api.py
+-rw-r--r--   0        0        0    18337 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runtime_api.py
+-rw-r--r--   0        0        0    12235 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/runtime_types_api.py
+-rw-r--r--   0        0        0    11900 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/teams_api.py
+-rw-r--r--   0        0        0    12201 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/transactions_api.py
+-rw-r--r--   0        0        0    23783 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api/users_api.py
+-rw-r--r--   0        0        0    27902 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/api_client.py
+-rw-r--r--   0        0        0    17035 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/configuration.py
+-rw-r--r--   0        0        0      591 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/Algorithm.md
+-rw-r--r--   0        0        0      570 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmIn.md
+-rw-r--r--   0        0        0      308 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmType.md
+-rw-r--r--   0        0        0    14024 2023-06-01 06:03:48.652898 qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmsApi.md
+-rw-r--r--   0        0        0      900 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRun.md
+-rw-r--r--   0        0        0      353 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunIn.md
+-rw-r--r--   0        0        0      309 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunStatus.md
+-rw-r--r--   0        0        0    20148 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRunsApi.md
+-rw-r--r--   0        0        0      445 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Commit.md
+-rw-r--r--   0        0        0      377 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CommitIn.md
+-rw-r--r--   0        0        0    11154 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CommitsApi.md
+-rw-r--r--   0        0        0      307 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/CompileStage.md
+-rw-r--r--   0        0        0      301 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Domain.md
+-rw-r--r--   0        0        0      678 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/File.md
+-rw-r--r--   0        0        0      668 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FileIn.md
+-rw-r--r--   0        0        0    10940 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FilesApi.md
+-rw-r--r--   0        0        0      434 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResult.md
+-rw-r--r--   0        0        0      366 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResultIn.md
+-rw-r--r--   0        0        0     9712 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/FinalResultsApi.md
+-rw-r--r--   0        0        0      323 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/HTTPNotFoundError.md
+-rw-r--r--   0        0        0      376 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/HTTPValidationError.md
+-rw-r--r--   0        0        0      363 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Language.md
+-rw-r--r--   0        0        0     4893 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/LanguagesApi.md
+-rw-r--r--   0        0        0      292 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/LocationInner.md
+-rw-r--r--   0        0        0      498 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Member.md
+-rw-r--r--   0        0        0      477 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MemberIn.md
+-rw-r--r--   0        0        0     9315 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MembersApi.md
+-rw-r--r--   0        0        0      427 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Metadata.md
+-rw-r--r--   0        0        0     7574 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MetadataApi.md
+-rw-r--r--   0        0        0      359 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/MetadataIn.md
+-rw-r--r--   0        0        0      368 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Permission.md
+-rw-r--r--   0        0        0      342 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionGroup.md
+-rw-r--r--   0        0        0     9721 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionsApi.md
+-rw-r--r--   0        0        0      500 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Project.md
+-rw-r--r--   0        0        0      432 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectIn.md
+-rw-r--r--   0        0        0      468 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectPatch.md
+-rw-r--r--   0        0        0    14529 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ProjectsApi.md
+-rw-r--r--   0        0        0      555 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Reservation.md
+-rw-r--r--   0        0        0      428 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationIn.md
+-rw-r--r--   0        0        0     9962 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationsApi.md
+-rw-r--r--   0        0        0      630 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Result.md
+-rw-r--r--   0        0        0      562 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ResultIn.md
+-rw-r--r--   0        0        0     9217 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ResultsApi.md
+-rw-r--r--   0        0        0      299 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Role.md
+-rw-r--r--   0        0        0      792 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Run.md
+-rw-r--r--   0        0        0      535 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunIn.md
+-rw-r--r--   0        0        0      304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunStatus.md
+-rw-r--r--   0        0        0    13158 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RunsApi.md
+-rw-r--r--   0        0        0      599 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Runtime.md
+-rw-r--r--   0        0        0     7110 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeApi.md
+-rw-r--r--   0        0        0      308 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeStatus.md
+-rw-r--r--   0        0        0      617 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeType.md
+-rw-r--r--   0        0        0     4904 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeTypesApi.md
+-rw-r--r--   0        0        0      657 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeWithAuthentication.md
+-rw-r--r--   0        0        0      304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ShareType.md
+-rw-r--r--   0        0        0      422 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Team.md
+-rw-r--r--   0        0        0     4544 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/TeamsApi.md
+-rw-r--r--   0        0        0      609 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/Transaction.md
+-rw-r--r--   0        0        0     4873 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/TransactionsApi.md
+-rw-r--r--   0        0        0      607 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/User.md
+-rw-r--r--   0        0        0      586 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/UserIn.md
+-rw-r--r--   0        0        0     9119 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/UsersApi.md
+-rw-r--r--   0        0        0      403 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/docs/ValidationError.md
+-rw-r--r--   0        0        0     5143 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/exceptions.py
+-rw-r--r--   0        0        0     3073 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/__init__.py
+-rw-r--r--   0        0        0     8684 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm.py
+-rw-r--r--   0        0        0     7545 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_in.py
+-rw-r--r--   0        0        0     3195 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_type.py
+-rw-r--r--   0        0        0    14456 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run.py
+-rw-r--r--   0        0        0     5910 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_in.py
+-rw-r--r--   0        0        0     3304 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_status.py
+-rw-r--r--   0        0        0     8312 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/commit.py
+-rw-r--r--   0        0        0     6318 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/commit_in.py
+-rw-r--r--   0        0        0     3275 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/compile_stage.py
+-rw-r--r--   0        0        0     3215 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/domain.py
+-rw-r--r--   0        0        0    10593 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/file.py
+-rw-r--r--   0        0        0     9327 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/file_in.py
+-rw-r--r--   0        0        0     7123 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/final_result.py
+-rw-r--r--   0        0        0     5081 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/final_result_in.py
+-rw-r--r--   0        0        0     3868 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/http_not_found_error.py
+-rw-r--r--   0        0        0     3782 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     6196 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/language.py
+-rw-r--r--   0        0        0     3052 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/location_inner.py
+-rw-r--r--   0        0        0     8530 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/member.py
+-rw-r--r--   0        0        0     7403 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/member_in.py
+-rw-r--r--   0        0        0     7015 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/metadata.py
+-rw-r--r--   0        0        0     4997 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/metadata_in.py
+-rw-r--r--   0        0        0     6303 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/permission.py
+-rw-r--r--   0        0        0     5248 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/permission_group.py
+-rw-r--r--   0        0        0     8855 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project.py
+-rw-r--r--   0        0        0     6861 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project_in.py
+-rw-r--r--   0        0        0     6448 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/project_patch.py
+-rw-r--r--   0        0        0    10862 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/reservation.py
+-rw-r--r--   0        0        0     7732 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/reservation_in.py
+-rw-r--r--   0        0        0    13635 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/result.py
+-rw-r--r--   0        0        0    11673 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/result_in.py
+-rw-r--r--   0        0        0     3153 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/role.py
+-rw-r--r--   0        0        0    11632 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run.py
+-rw-r--r--   0        0        0     6879 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run_in.py
+-rw-r--r--   0        0        0     3290 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/run_status.py
+-rw-r--r--   0        0        0     9940 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime.py
+-rw-r--r--   0        0        0     3273 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_status.py
+-rw-r--r--   0        0        0    11585 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_type.py
+-rw-r--r--   0        0        0    11844 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/runtime_with_authentication.py
+-rw-r--r--   0        0        0     3212 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/share_type.py
+-rw-r--r--   0        0        0     6842 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/team.py
+-rw-r--r--   0        0        0    10913 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/transaction.py
+-rw-r--r--   0        0        0     8950 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/user.py
+-rw-r--r--   0        0        0     7847 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/user_in.py
+-rw-r--r--   0        0        0     5308 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/models/validation_error.py
+-rw-r--r--   0        0        0     9931 2023-06-01 06:03:48.656899 qi_compute_api_client-0.4.0/compute_api_client/rest.py
+-rw-r--r--   0        0        0     1094 2023-06-01 06:04:01.248895 qi_compute_api_client-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    17438 1970-01-01 00:00:00.000000 qi_compute_api_client-0.4.0/PKG-INFO
```

### Comparing `qi_compute_api_client-0.1.0/LICENSE.md` & `qi_compute_api_client-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/README.md` & `qi_compute_api_client-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,25 +37,35 @@
 
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient(configuration) as api_client:
+async with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.AlgorithmsApi(api_client)
     algorithm_in = compute_api_client.AlgorithmIn() # AlgorithmIn | 
 
     try:
         # Create algorithm
-        api_response = api_instance.create_algorithm_algorithms_post(algorithm_in)
+        api_response = await api_instance.create_algorithm_algorithms_post(algorithm_in)
         pprint(api_response)
     except ApiException as e:
         print("Exception when calling AlgorithmsApi->create_algorithm_algorithms_post: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
@@ -113,14 +123,15 @@
 *ResultsApi* | [**read_result_results_id_get**](compute_api_client/docs/ResultsApi.md#read_result_results_id_get) | **GET** /results/{id} | Retrieve result
 *ResultsApi* | [**read_results_by_run_id_results_run_run_id_get**](compute_api_client/docs/ResultsApi.md#read_results_by_run_id_results_run_run_id_get) | **GET** /results/run/{run_id} | Retrieve result
 *RunsApi* | [**create_run_runs_post**](compute_api_client/docs/RunsApi.md#create_run_runs_post) | **POST** /runs | Create run
 *RunsApi* | [**delete_run_runs_id_delete**](compute_api_client/docs/RunsApi.md#delete_run_runs_id_delete) | **DELETE** /runs/{id} | Destroy run
 *RunsApi* | [**read_run_runs_id_get**](compute_api_client/docs/RunsApi.md#read_run_runs_id_get) | **GET** /runs/{id} | Retrieve run
 *RunsApi* | [**read_runs_runs_get**](compute_api_client/docs/RunsApi.md#read_runs_runs_get) | **GET** /runs | List runs
 *RunsApi* | [**start_run_runs_id_start_patch**](compute_api_client/docs/RunsApi.md#start_run_runs_id_start_patch) | **PATCH** /runs/{id}/start | Start run
+*RuntimeApi* | [**create_runtime_runtimes_post**](compute_api_client/docs/RuntimeApi.md#create_runtime_runtimes_post) | **POST** /runtimes | Create runtime
 *RuntimeApi* | [**read_runtime_runtimes_id_get**](compute_api_client/docs/RuntimeApi.md#read_runtime_runtimes_id_get) | **GET** /runtimes/{id} | Retrieve runtime
 *RuntimeApi* | [**read_runtimes_runtimes_get**](compute_api_client/docs/RuntimeApi.md#read_runtimes_runtimes_get) | **GET** /runtimes | List runtimes
 *RuntimeTypesApi* | [**read_runtime_type_runtime_types_id_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_type_runtime_types_id_get) | **GET** /runtime_types/{id} | Retrieve runtime type
 *RuntimeTypesApi* | [**read_runtime_types_runtime_types_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_types_runtime_types_get) | **GET** /runtime_types/ | List runtime types
 *TeamsApi* | [**read_team_teams_id_get**](compute_api_client/docs/TeamsApi.md#read_team_teams_id_get) | **GET** /teams/{id} | Retrieve teams
 *TeamsApi* | [**read_teams_teams_get**](compute_api_client/docs/TeamsApi.md#read_teams_teams_get) | **GET** /teams/ | List teams
 *TransactionsApi* | [**read_transaction_transactions_id_get**](compute_api_client/docs/TransactionsApi.md#read_transaction_transactions_id_get) | **GET** /transactions/{id} | Retrieve transactions
@@ -167,24 +178,38 @@
  - [Role](compute_api_client/docs/Role.md)
  - [Run](compute_api_client/docs/Run.md)
  - [RunIn](compute_api_client/docs/RunIn.md)
  - [RunStatus](compute_api_client/docs/RunStatus.md)
  - [Runtime](compute_api_client/docs/Runtime.md)
  - [RuntimeStatus](compute_api_client/docs/RuntimeStatus.md)
  - [RuntimeType](compute_api_client/docs/RuntimeType.md)
+ - [RuntimeWithAuthentication](compute_api_client/docs/RuntimeWithAuthentication.md)
  - [ShareType](compute_api_client/docs/ShareType.md)
  - [Team](compute_api_client/docs/Team.md)
  - [Transaction](compute_api_client/docs/Transaction.md)
  - [User](compute_api_client/docs/User.md)
  - [UserIn](compute_api_client/docs/UserIn.md)
  - [ValidationError](compute_api_client/docs/ValidationError.md)
 
 
 ## Documentation For Authorization
 
- All endpoints do not require authorization.
+
+## user
+
+- **Type**: API key
+- **API key parameter name**: X-userid
+- **Location**: HTTP header
+
+
+## runtime
+
+- **Type**: API key
+- **API key parameter name**: Authorization
+- **Location**: HTTP header
+
 
 ## Author
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/__init__.py` & `qi_compute_api_client-0.4.0/compute_api_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 from compute_api_client.models.role import Role
 from compute_api_client.models.run import Run
 from compute_api_client.models.run_in import RunIn
 from compute_api_client.models.run_status import RunStatus
 from compute_api_client.models.runtime import Runtime
 from compute_api_client.models.runtime_status import RuntimeStatus
 from compute_api_client.models.runtime_type import RuntimeType
+from compute_api_client.models.runtime_with_authentication import RuntimeWithAuthentication
 from compute_api_client.models.share_type import ShareType
 from compute_api_client.models.team import Team
 from compute_api_client.models.transaction import Transaction
 from compute_api_client.models.user import User
 from compute_api_client.models.user_in import UserIn
 from compute_api_client.models.validation_error import ValidationError
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/__init__.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/algorithms_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/algorithms_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Algorithm",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/algorithms/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "Algorithm",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Algorithm]",
         }
 
         return self.api_client.call_api(
             '/algorithms', 'GET',
@@ -711,15 +711,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'PUT', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Algorithm",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/batch_runs_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/batch_runs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "BatchRun",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -431,15 +431,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -578,15 +578,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'PATCH', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -706,15 +706,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "BatchRun",
             404: "HTTPNotFoundError",
         }
 
         return self.api_client.call_api(
@@ -834,15 +834,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[BatchRun]",
         }
 
         return self.api_client.call_api(
             '/batch_runs', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/commits_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/commits_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Commit",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/commits/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "Commit",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Commit]",
         }
 
         return self.api_client.call_api(
             '/commits', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/files_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/files_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "File",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/files/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "File",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[File]",
         }
 
         return self.api_client.call_api(
             '/files', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/final_results_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/final_results_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             201: "FinalResult",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "FinalResult",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -430,15 +430,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "FinalResult",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/languages_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/languages_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Language",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -282,15 +282,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Language]",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/members_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/members_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Member",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/members/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Member",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Member]",
         }
 
         return self.api_client.call_api(
             '/members', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/metadata_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Metadata",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Metadata]",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -430,15 +430,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Metadata",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/permissions_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/permissions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "PermissionGroup",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -275,15 +275,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[PermissionGroup]",
         }
 
         return self.api_client.call_api(
             '/permission_groups/', 'GET',
@@ -412,15 +412,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Permission",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -541,15 +541,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Permission]",
         }
 
         return self.api_client.call_api(
             '/permissions/', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/projects_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Project",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/projects/{id}', 'DELETE',
             path_params,
             query_params,
@@ -445,15 +445,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'PATCH', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Project",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -584,15 +584,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Project",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -713,15 +713,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Project]",
         }
 
         return self.api_client.call_api(
             '/projects', 'GET',
@@ -868,15 +868,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'PUT', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Project",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/reservations_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/reservations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Reservation",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Reservation",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -421,15 +421,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Reservation]",
         }
 
         return self.api_client.call_api(
             '/reservations', 'GET',
@@ -558,15 +558,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Reservation",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/results_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/results_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             201: "Result",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Result",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -431,15 +431,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Result]",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/runs_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/runs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "Run",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/runs/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Run",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Run]",
         }
 
         return self.api_client.call_api(
             '/runs', 'GET',
@@ -693,15 +693,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['runtime', 'user']  # noqa: E501
 
         response_types_map = {
             200: "Run",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/runtime_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/runtime_types_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 from compute_api_client.api_client import ApiClient
 from compute_api_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class RuntimeApi(object):
+class RuntimeTypesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def read_runtime_runtimes_id_get(self, id, **kwargs):  # noqa: E501
-        """Retrieve runtime  # noqa: E501
+    def read_runtime_type_runtime_types_id_get(self, id, **kwargs):  # noqa: E501
+        """Retrieve runtime type  # noqa: E501
 
-        Get runtime by ID.  # noqa: E501
+        Get runtime type by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_runtimes_id_get(id, async_req=True)
+        >>> thread = api.read_runtime_type_runtime_types_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -57,27 +57,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Runtime
+        :rtype: RuntimeType
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_runtime_runtimes_id_get_with_http_info(id, **kwargs)  # noqa: E501
+        return self.read_runtime_type_runtime_types_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
-    def read_runtime_runtimes_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Retrieve runtime  # noqa: E501
+    def read_runtime_type_runtime_types_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Retrieve runtime type  # noqa: E501
 
-        Get runtime by ID.  # noqa: E501
+        Get runtime type by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_runtimes_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.read_runtime_type_runtime_types_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -95,15 +95,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Runtime, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(RuntimeType, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'id'
         ]
@@ -119,21 +119,21 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_runtime_runtimes_id_get" % key
+                    " to method read_runtime_type_runtime_types_id_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and local_var_params.get('id') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `read_runtime_runtimes_id_get`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `read_runtime_type_runtime_types_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -146,24 +146,24 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "Runtime",
+            200: "RuntimeType",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/runtimes/{id}', 'GET',
+            '/runtime_types/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -171,22 +171,22 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def read_runtimes_runtimes_get(self, **kwargs):  # noqa: E501
-        """List runtimes  # noqa: E501
+    def read_runtime_types_runtime_types_get(self, **kwargs):  # noqa: E501
+        """List runtime types  # noqa: E501
 
-        Read runtimes.  # noqa: E501
+        Read runtime types.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtimes_runtimes_get(async_req=True)
+        >>> thread = api.read_runtime_types_runtime_types_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -194,27 +194,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[Runtime]
+        :rtype: list[RuntimeType]
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_runtimes_runtimes_get_with_http_info(**kwargs)  # noqa: E501
+        return self.read_runtime_types_runtime_types_get_with_http_info(**kwargs)  # noqa: E501
 
-    def read_runtimes_runtimes_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List runtimes  # noqa: E501
+    def read_runtime_types_runtime_types_get_with_http_info(self, **kwargs):  # noqa: E501
+        """List runtime types  # noqa: E501
 
-        Read runtimes.  # noqa: E501
+        Read runtime types.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtimes_runtimes_get_with_http_info(async_req=True)
+        >>> thread = api.read_runtime_types_runtime_types_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -230,15 +230,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[Runtime], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[RuntimeType], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
         ]
         all_params.extend(
@@ -253,15 +253,15 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_runtimes_runtimes_get" % key
+                    " to method read_runtime_types_runtime_types_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -275,22 +275,22 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "list[Runtime]",
+            200: "list[RuntimeType]",
         }
 
         return self.api_client.call_api(
-            '/runtimes', 'GET',
+            '/runtime_types/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/runtime_types_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/transactions_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 from compute_api_client.api_client import ApiClient
 from compute_api_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class RuntimeTypesApi(object):
+class TransactionsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def read_runtime_type_runtime_types_id_get(self, id, **kwargs):  # noqa: E501
-        """Retrieve runtime type  # noqa: E501
+    def read_transaction_transactions_id_get(self, id, **kwargs):  # noqa: E501
+        """Retrieve transactions  # noqa: E501
 
-        Get runtime type by ID.  # noqa: E501
+        Get transaction by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_type_runtime_types_id_get(id, async_req=True)
+        >>> thread = api.read_transaction_transactions_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -57,27 +57,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: RuntimeType
+        :rtype: Transaction
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_runtime_type_runtime_types_id_get_with_http_info(id, **kwargs)  # noqa: E501
+        return self.read_transaction_transactions_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
-    def read_runtime_type_runtime_types_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Retrieve runtime type  # noqa: E501
+    def read_transaction_transactions_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Retrieve transactions  # noqa: E501
 
-        Get runtime type by ID.  # noqa: E501
+        Get transaction by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_type_runtime_types_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.read_transaction_transactions_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -95,15 +95,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(RuntimeType, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Transaction, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'id'
         ]
@@ -119,21 +119,21 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_runtime_type_runtime_types_id_get" % key
+                    " to method read_transaction_transactions_id_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and local_var_params.get('id') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `read_runtime_type_runtime_types_id_get`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `read_transaction_transactions_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -146,24 +146,24 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "RuntimeType",
+            200: "Transaction",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/runtime_types/{id}', 'GET',
+            '/transactions/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -171,22 +171,22 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def read_runtime_types_runtime_types_get(self, **kwargs):  # noqa: E501
-        """List runtime types  # noqa: E501
+    def read_transactions_transactions_get(self, **kwargs):  # noqa: E501
+        """List transactions  # noqa: E501
 
-        Read runtime types.  # noqa: E501
+        Read transactions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_types_runtime_types_get(async_req=True)
+        >>> thread = api.read_transactions_transactions_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -194,27 +194,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[RuntimeType]
+        :rtype: list[Transaction]
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_runtime_types_runtime_types_get_with_http_info(**kwargs)  # noqa: E501
+        return self.read_transactions_transactions_get_with_http_info(**kwargs)  # noqa: E501
 
-    def read_runtime_types_runtime_types_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List runtime types  # noqa: E501
+    def read_transactions_transactions_get_with_http_info(self, **kwargs):  # noqa: E501
+        """List transactions  # noqa: E501
 
-        Read runtime types.  # noqa: E501
+        Read transactions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_runtime_types_runtime_types_get_with_http_info(async_req=True)
+        >>> thread = api.read_transactions_transactions_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -230,15 +230,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[RuntimeType], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Transaction], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
         ]
         all_params.extend(
@@ -253,15 +253,15 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_runtime_types_runtime_types_get" % key
+                    " to method read_transactions_transactions_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -275,22 +275,22 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "list[RuntimeType]",
+            200: "list[Transaction]",
         }
 
         return self.api_client.call_api(
-            '/runtime_types/', 'GET',
+            '/transactions/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/teams_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/teams_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "Team",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -275,15 +275,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[Team]",
         }
 
         return self.api_client.call_api(
             '/teams/', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/transactions_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/runtime_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,34 +20,180 @@
 from compute_api_client.api_client import ApiClient
 from compute_api_client.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TransactionsApi(object):
+class RuntimeApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def read_transaction_transactions_id_get(self, id, **kwargs):  # noqa: E501
-        """Retrieve transactions  # noqa: E501
+    def create_runtime_runtimes_post(self, runtime, **kwargs):  # noqa: E501
+        """Create runtime  # noqa: E501
 
-        Get transaction by ID.  # noqa: E501
+        Create new runtime.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_transaction_transactions_id_get(id, async_req=True)
+        >>> thread = api.create_runtime_runtimes_post(runtime, async_req=True)
+        >>> result = thread.get()
+
+        :param runtime: (required)
+        :type runtime: Runtime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: RuntimeWithAuthentication
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.create_runtime_runtimes_post_with_http_info(runtime, **kwargs)  # noqa: E501
+
+    def create_runtime_runtimes_post_with_http_info(self, runtime, **kwargs):  # noqa: E501
+        """Create runtime  # noqa: E501
+
+        Create new runtime.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_runtime_runtimes_post_with_http_info(runtime, async_req=True)
+        >>> result = thread.get()
+
+        :param runtime: (required)
+        :type runtime: Runtime
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(RuntimeWithAuthentication, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'runtime'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_runtime_runtimes_post" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'runtime' is set
+        if self.api_client.client_side_validation and local_var_params.get('runtime') is None:  # noqa: E501
+            raise ApiValueError("Missing the required parameter `runtime` when calling `create_runtime_runtimes_post`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = dict(local_var_params.get('_headers', {}))
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'runtime' in local_var_params:
+            body_params = local_var_params['runtime']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        content_types_list = local_var_params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json'],
+                'POST', body_params))  # noqa: E501
+        if content_types_list:
+                header_params['Content-Type'] = content_types_list
+
+        # Authentication setting
+        auth_settings = ['user']  # noqa: E501
+
+        response_types_map = {
+            201: "RuntimeWithAuthentication",
+            422: "HTTPValidationError",
+        }
+
+        return self.api_client.call_api(
+            '/runtimes', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_types_map=response_types_map,
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats,
+            _request_auth=local_var_params.get('_request_auth'))
+
+    def read_runtime_runtimes_id_get(self, id, **kwargs):  # noqa: E501
+        """Retrieve runtime  # noqa: E501
+
+        Get runtime by ID.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.read_runtime_runtimes_id_get(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -57,27 +203,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Transaction
+        :rtype: Runtime
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_transaction_transactions_id_get_with_http_info(id, **kwargs)  # noqa: E501
+        return self.read_runtime_runtimes_id_get_with_http_info(id, **kwargs)  # noqa: E501
 
-    def read_transaction_transactions_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
-        """Retrieve transactions  # noqa: E501
+    def read_runtime_runtimes_id_get_with_http_info(self, id, **kwargs):  # noqa: E501
+        """Retrieve runtime  # noqa: E501
 
-        Get transaction by ID.  # noqa: E501
+        Get runtime by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_transaction_transactions_id_get_with_http_info(id, async_req=True)
+        >>> thread = api.read_runtime_runtimes_id_get_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -95,15 +241,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Transaction, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Runtime, status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
             'id'
         ]
@@ -119,21 +265,21 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_transaction_transactions_id_get" % key
+                    " to method read_runtime_runtimes_id_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
         # verify the required parameter 'id' is set
         if self.api_client.client_side_validation and local_var_params.get('id') is None:  # noqa: E501
-            raise ApiValueError("Missing the required parameter `id` when calling `read_transaction_transactions_id_get`")  # noqa: E501
+            raise ApiValueError("Missing the required parameter `id` when calling `read_runtime_runtimes_id_get`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
@@ -146,24 +292,24 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "Transaction",
+            200: "Runtime",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
-            '/transactions/{id}', 'GET',
+            '/runtimes/{id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
@@ -171,22 +317,22 @@
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats,
             _request_auth=local_var_params.get('_request_auth'))
 
-    def read_transactions_transactions_get(self, **kwargs):  # noqa: E501
-        """List transactions  # noqa: E501
+    def read_runtimes_runtimes_get(self, **kwargs):  # noqa: E501
+        """List runtimes  # noqa: E501
 
-        Read transactions.  # noqa: E501
+        Read runtimes.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_transactions_transactions_get(async_req=True)
+        >>> thread = api.read_runtimes_runtimes_get(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -194,27 +340,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: list[Transaction]
+        :rtype: list[Runtime]
         """
         kwargs['_return_http_data_only'] = True
-        return self.read_transactions_transactions_get_with_http_info(**kwargs)  # noqa: E501
+        return self.read_runtimes_runtimes_get_with_http_info(**kwargs)  # noqa: E501
 
-    def read_transactions_transactions_get_with_http_info(self, **kwargs):  # noqa: E501
-        """List transactions  # noqa: E501
+    def read_runtimes_runtimes_get_with_http_info(self, **kwargs):  # noqa: E501
+        """List runtimes  # noqa: E501
 
-        Read transactions.  # noqa: E501
+        Read runtimes.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.read_transactions_transactions_get_with_http_info(async_req=True)
+        >>> thread = api.read_runtimes_runtimes_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -230,15 +376,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(list[Transaction], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(list[Runtime], status_code(int), headers(HTTPHeaderDict))
         """
 
         local_var_params = locals()
 
         all_params = [
         ]
         all_params.extend(
@@ -253,15 +399,15 @@
             ]
         )
 
         for key, val in six.iteritems(local_var_params['kwargs']):
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method read_transactions_transactions_get" % key
+                    " to method read_runtimes_runtimes_get" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
@@ -275,22 +421,22 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
-            200: "list[Transaction]",
+            200: "list[Runtime]",
         }
 
         return self.api_client.call_api(
-            '/transactions/', 'GET',
+            '/runtimes', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_types_map=response_types_map,
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api/users_api.py` & `qi_compute_api_client-0.4.0/compute_api_client/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             self.api_client.select_header_content_type(
                 ['application/json'],
                 'POST', body_params))  # noqa: E501
         if content_types_list:
                 header_params['Content-Type'] = content_types_list
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             201: "User",
             422: "HTTPValidationError",
         }
 
         return self.api_client.call_api(
@@ -292,15 +292,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
             '/users/{id}', 'DELETE',
             path_params,
             query_params,
@@ -427,15 +427,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "User",
             404: "HTTPNotFoundError",
             422: "HTTPValidationError",
         }
 
@@ -556,15 +556,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = []  # noqa: E501
+        auth_settings = ['user']  # noqa: E501
 
         response_types_map = {
             200: "list[User]",
         }
 
         return self.api_client.call_api(
             '/users', 'GET',
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/api_client.py` & `qi_compute_api_client-0.4.0/compute_api_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,16 +298,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict('):
-                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
+            if klass.startswith('dict['):
+                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -688,14 +688,15 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
+        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/configuration.py` & `qi_compute_api_client-0.4.0/compute_api_client/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,34 @@
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
     :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
       in PEM format
 
+    :Example:
+
+    API Key Authentication Example.
+    Given the following security scheme in the OpenAPI specification:
+      components:
+        securitySchemes:
+          cookieAuth:         # name for the security scheme
+            type: apiKey
+            in: cookie
+            name: JSESSIONID  # cookie name
+
+    You can programmatically set the cookie:
+
+conf = compute_api_client.Configuration(
+    api_key={'cookieAuth': 'abc123'}
+    api_key_prefix={'cookieAuth': 'JSESSIONID'}
+)
+
+    The following cookie will be added to the HTTP request:
+       Cookie: JSESSIONID abc123
     """
 
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
@@ -362,14 +382,32 @@
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         auth = {}
+        if 'user' in self.api_key:
+            auth['user'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'X-userid',
+                'value': self.get_api_key_with_prefix(
+                    'user',
+                ),
+            }
+        if 'runtime' in self.api_key:
+            auth['runtime'] = {
+                'type': 'api_key',
+                'in': 'header',
+                'key': 'Authorization',
+                'value': self.get_api_key_with_prefix(
+                    'runtime',
+                ),
+            }
         return auth
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Algorithm.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Algorithm.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/AlgorithmIn.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/AlgorithmIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/AlgorithmsApi.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/ReservationsApi.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,195 +1,153 @@
-# compute_api_client.AlgorithmsApi
+# compute_api_client.ReservationsApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**create_algorithm_algorithms_post**](AlgorithmsApi.md#create_algorithm_algorithms_post) | **POST** /algorithms | Create algorithm
-[**delete_algorithm_algorithms_id_delete**](AlgorithmsApi.md#delete_algorithm_algorithms_id_delete) | **DELETE** /algorithms/{id} | Destroy algorithm
-[**read_algorithm_algorithms_id_get**](AlgorithmsApi.md#read_algorithm_algorithms_id_get) | **GET** /algorithms/{id} | Retrieve algorithm
-[**read_algorithms_algorithms_get**](AlgorithmsApi.md#read_algorithms_algorithms_get) | **GET** /algorithms | List algorithms
-[**update_algorithm_algorithms_id_put**](AlgorithmsApi.md#update_algorithm_algorithms_id_put) | **PUT** /algorithms/{id} | Update algorithm
+[**create_reservation_reservations_post**](ReservationsApi.md#create_reservation_reservations_post) | **POST** /reservations | Create reservation
+[**read_reservation_reservations_id_get**](ReservationsApi.md#read_reservation_reservations_id_get) | **GET** /reservations/{id} | Retrieve reservation
+[**read_reservations_reservations_get**](ReservationsApi.md#read_reservations_reservations_get) | **GET** /reservations | List reservations
+[**terminate_reservation_reservations_id_terminate_patch**](ReservationsApi.md#terminate_reservation_reservations_id_terminate_patch) | **PATCH** /reservations/{id}/terminate | Terminate reservation
 
 
-# **create_algorithm_algorithms_post**
-> Algorithm create_algorithm_algorithms_post(algorithm_in)
+# **create_reservation_reservations_post**
+> Reservation create_reservation_reservations_post(reservation_in)
 
-Create algorithm
+Create reservation
 
-Create new algorithm.
+Create new reservation.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.AlgorithmsApi(api_client)
-    algorithm_in = compute_api_client.AlgorithmIn() # AlgorithmIn | 
+    api_instance = compute_api_client.ReservationsApi(api_client)
+    reservation_in = compute_api_client.ReservationIn() # ReservationIn | 
 
     try:
-        # Create algorithm
-        api_response = api_instance.create_algorithm_algorithms_post(algorithm_in)
+        # Create reservation
+        api_response = api_instance.create_reservation_reservations_post(reservation_in)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AlgorithmsApi->create_algorithm_algorithms_post: %s\n" % e)
+        print("Exception when calling ReservationsApi->create_reservation_reservations_post: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **algorithm_in** | [**AlgorithmIn**](AlgorithmIn.md)|  | 
+ **reservation_in** | [**ReservationIn**](ReservationIn.md)|  | 
 
 ### Return type
 
-[**Algorithm**](Algorithm.md)
+[**Reservation**](Reservation.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: application/json
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **201** | Successful Response |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **delete_algorithm_algorithms_id_delete**
-> delete_algorithm_algorithms_id_delete(id)
+# **read_reservation_reservations_id_get**
+> Reservation read_reservation_reservations_id_get(id)
 
-Destroy algorithm
+Retrieve reservation
 
-Delete an algorithm.
+Get reservation by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
 
-# Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
-    # Create an instance of the API class
-    api_instance = compute_api_client.AlgorithmsApi(api_client)
-    id = 56 # int | 
-
-    try:
-        # Destroy algorithm
-        api_instance.delete_algorithm_algorithms_id_delete(id)
-    except ApiException as e:
-        print("Exception when calling AlgorithmsApi->delete_algorithm_algorithms_id_delete: %s\n" % e)
-```
-
-### Parameters
-
-Name | Type | Description  | Notes
-------------- | ------------- | ------------- | -------------
- **id** | **int**|  | 
-
-### Return type
-
-void (empty response body)
-
-### Authorization
-
-No authorization required
-
-### HTTP request headers
-
- - **Content-Type**: Not defined
- - **Accept**: application/json
-
-### HTTP response details
-| Status code | Description | Response headers |
-|-------------|-------------|------------------|
-**204** | Successful Response |  -  |
-**404** | Not Found |  -  |
-**422** | Validation Error |  -  |
-
-[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
-
-# **read_algorithm_algorithms_id_get**
-> Algorithm read_algorithm_algorithms_id_get(id)
-
-Retrieve algorithm
-
-Get algorithm by ID.
-
-### Example
-
-```python
-from __future__ import print_function
-import time
-import compute_api_client
-from compute_api_client.rest import ApiException
-from pprint import pprint
-# Defining the host is optional and defaults to http://localhost
-# See configuration.py for a list of all supported configuration parameters.
-configuration = compute_api_client.Configuration(
-    host = "http://localhost"
-)
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
 
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.AlgorithmsApi(api_client)
+    api_instance = compute_api_client.ReservationsApi(api_client)
     id = 56 # int | 
 
     try:
-        # Retrieve algorithm
-        api_response = api_instance.read_algorithm_algorithms_id_get(id)
+        # Retrieve reservation
+        api_response = api_instance.read_reservation_reservations_id_get(id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AlgorithmsApi->read_algorithm_algorithms_id_get: %s\n" % e)
+        print("Exception when calling ReservationsApi->read_reservation_reservations_id_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **id** | **int**|  | 
 
 ### Return type
 
-[**Algorithm**](Algorithm.md)
+[**Reservation**](Reservation.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -197,127 +155,147 @@
 |-------------|-------------|------------------|
 **200** | Successful Response |  -  |
 **404** | Not Found |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **read_algorithms_algorithms_get**
-> list[Algorithm] read_algorithms_algorithms_get()
+# **read_reservations_reservations_get**
+> list[Reservation] read_reservations_reservations_get()
 
-List algorithms
+List reservations
 
-List algorithms.
+Read reservations.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.AlgorithmsApi(api_client)
+    api_instance = compute_api_client.ReservationsApi(api_client)
     
     try:
-        # List algorithms
-        api_response = api_instance.read_algorithms_algorithms_get()
+        # List reservations
+        api_response = api_instance.read_reservations_reservations_get()
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AlgorithmsApi->read_algorithms_algorithms_get: %s\n" % e)
+        print("Exception when calling ReservationsApi->read_reservations_reservations_get: %s\n" % e)
 ```
 
 ### Parameters
 This endpoint does not need any parameter.
 
 ### Return type
 
-[**list[Algorithm]**](Algorithm.md)
+[**list[Reservation]**](Reservation.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Successful Response |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **update_algorithm_algorithms_id_put**
-> Algorithm update_algorithm_algorithms_id_put(id, algorithm_in)
+# **terminate_reservation_reservations_id_terminate_patch**
+> Reservation terminate_reservation_reservations_id_terminate_patch(id)
 
-Update algorithm
+Terminate reservation
 
-Update an algorithm.
+Terminate reservation by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.AlgorithmsApi(api_client)
+    api_instance = compute_api_client.ReservationsApi(api_client)
     id = 56 # int | 
-algorithm_in = compute_api_client.AlgorithmIn() # AlgorithmIn | 
 
     try:
-        # Update algorithm
-        api_response = api_instance.update_algorithm_algorithms_id_put(id, algorithm_in)
+        # Terminate reservation
+        api_response = api_instance.terminate_reservation_reservations_id_terminate_patch(id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AlgorithmsApi->update_algorithm_algorithms_id_put: %s\n" % e)
+        print("Exception when calling ReservationsApi->terminate_reservation_reservations_id_terminate_patch: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **id** | **int**|  | 
- **algorithm_in** | [**AlgorithmIn**](AlgorithmIn.md)|  | 
 
 ### Return type
 
-[**Algorithm**](Algorithm.md)
+[**Reservation**](Reservation.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
- - **Content-Type**: application/json
+ - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **200** | Successful Response |  -  |
 **404** | Not Found |  -  |
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/BatchRun.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/BatchRun.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/File.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/File.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/FileIn.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/FileIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/FilesApi.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/UsersApi.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,152 @@
-# compute_api_client.FilesApi
+# compute_api_client.UsersApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**create_file_files_post**](FilesApi.md#create_file_files_post) | **POST** /files | Create file
-[**delete_file_files_id_delete**](FilesApi.md#delete_file_files_id_delete) | **DELETE** /files/{id} | Destroy file
-[**read_file_files_id_get**](FilesApi.md#read_file_files_id_get) | **GET** /files/{id} | Retrieve file
-[**read_files_files_get**](FilesApi.md#read_files_files_get) | **GET** /files | List files
+[**create_user_users_post**](UsersApi.md#create_user_users_post) | **POST** /users | Create user
+[**delete_user_users_id_delete**](UsersApi.md#delete_user_users_id_delete) | **DELETE** /users/{id} | Destroy user
+[**read_user_users_id_get**](UsersApi.md#read_user_users_id_get) | **GET** /users/{id} | Retrieve user
+[**read_users_users_get**](UsersApi.md#read_users_users_get) | **GET** /users | List users
 
 
-# **create_file_files_post**
-> File create_file_files_post(file_in)
+# **create_user_users_post**
+> User create_user_users_post(user_in)
 
-Create file
+Create user
 
-Create new file.
+Create new user.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.FilesApi(api_client)
-    file_in = compute_api_client.FileIn() # FileIn | 
+    api_instance = compute_api_client.UsersApi(api_client)
+    user_in = compute_api_client.UserIn() # UserIn | 
 
     try:
-        # Create file
-        api_response = api_instance.create_file_files_post(file_in)
+        # Create user
+        api_response = api_instance.create_user_users_post(user_in)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling FilesApi->create_file_files_post: %s\n" % e)
+        print("Exception when calling UsersApi->create_user_users_post: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
- **file_in** | [**FileIn**](FileIn.md)|  | 
+ **user_in** | [**UserIn**](UserIn.md)|  | 
 
 ### Return type
 
-[**File**](File.md)
+[**User**](User.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: application/json
  - **Accept**: application/json
 
 ### HTTP response details
 | Status code | Description | Response headers |
 |-------------|-------------|------------------|
 **201** | Successful Response |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **delete_file_files_id_delete**
-> delete_file_files_id_delete(id)
+# **delete_user_users_id_delete**
+> delete_user_users_id_delete(id)
 
-Destroy file
+Destroy user
 
-Delete a file.
+Delete a user.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.FilesApi(api_client)
+    api_instance = compute_api_client.UsersApi(api_client)
     id = 56 # int | 
 
     try:
-        # Destroy file
-        api_instance.delete_file_files_id_delete(id)
+        # Destroy user
+        api_instance.delete_user_users_id_delete(id)
     except ApiException as e:
-        print("Exception when calling FilesApi->delete_file_files_id_delete: %s\n" % e)
+        print("Exception when calling UsersApi->delete_user_users_id_delete: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **id** | **int**|  | 
 
 ### Return type
 
 void (empty response body)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -132,63 +154,74 @@
 |-------------|-------------|------------------|
 **204** | Successful Response |  -  |
 **404** | Not Found |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **read_file_files_id_get**
-> File read_file_files_id_get(id)
+# **read_user_users_id_get**
+> User read_user_users_id_get(id)
 
-Retrieve file
+Retrieve user
 
-Get file by ID.
+Get user by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.FilesApi(api_client)
+    api_instance = compute_api_client.UsersApi(api_client)
     id = 56 # int | 
 
     try:
-        # Retrieve file
-        api_response = api_instance.read_file_files_id_get(id)
+        # Retrieve user
+        api_response = api_instance.read_user_users_id_get(id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling FilesApi->read_file_files_id_get: %s\n" % e)
+        print("Exception when calling UsersApi->read_user_users_id_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **id** | **int**|  | 
 
 ### Return type
 
-[**File**](File.md)
+[**User**](User.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -196,59 +229,70 @@
 |-------------|-------------|------------------|
 **200** | Successful Response |  -  |
 **404** | Not Found |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **read_files_files_get**
-> list[File] read_files_files_get()
+# **read_users_users_get**
+> list[User] read_users_users_get()
 
-List files
+List users
 
-List files.
+Read users.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.FilesApi(api_client)
+    api_instance = compute_api_client.UsersApi(api_client)
     
     try:
-        # List files
-        api_response = api_instance.read_files_files_get()
+        # List users
+        api_response = api_instance.read_users_users_get()
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling FilesApi->read_files_files_get: %s\n" % e)
+        print("Exception when calling UsersApi->read_users_users_get: %s\n" % e)
 ```
 
 ### Parameters
 This endpoint does not need any parameter.
 
 ### Return type
 
-[**list[File]**](File.md)
+[**list[User]**](User.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/PermissionsApi.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/PermissionsApi.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,29 +15,40 @@
 
 Retrieve permission groups
 
 Get permission group by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.PermissionsApi(api_client)
     id = 56 # int | 
 
     try:
         # Retrieve permission groups
         api_response = api_instance.read_permission_group_permission_groups_id_get(id)
@@ -54,15 +65,15 @@
 
 ### Return type
 
 [**PermissionGroup**](PermissionGroup.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -79,29 +90,40 @@
 
 List permission groups
 
 Read permissions groups.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.PermissionsApi(api_client)
     
     try:
         # List permission groups
         api_response = api_instance.read_permission_groups_permission_groups_get()
         pprint(api_response)
@@ -114,15 +136,15 @@
 
 ### Return type
 
 [**list[PermissionGroup]**](PermissionGroup.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -137,29 +159,40 @@
 
 Retrieve permissions
 
 Get permission by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.PermissionsApi(api_client)
     id = 56 # int | 
 
     try:
         # Retrieve permissions
         api_response = api_instance.read_permission_permissions_id_get(id)
@@ -176,15 +209,15 @@
 
 ### Return type
 
 [**Permission**](Permission.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -201,29 +234,40 @@
 
 List permissions
 
 Read permissions.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.PermissionsApi(api_client)
     
     try:
         # List permissions
         api_response = api_instance.read_permissions_permissions_get()
         pprint(api_response)
@@ -236,15 +280,15 @@
 
 ### Return type
 
 [**list[Permission]**](Permission.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Reservation.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Reservation.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Result.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Result.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,16 @@
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **created_on** | **datetime** |  | [readonly] 
 **id** | **int** |  | 
 **number_of_qubits** | **int** |  | 
 **execution_time_in_seconds** | **float** |  | 
-**raw_text** | **str** |  | 
-**raw_data** | **object** |  | [optional] 
-**histogram** | **object** |  | [optional] 
-**measurement_mask** | **object** |  | [optional] 
-**quantum_states** | **object** |  | [optional] 
-**measurement_register** | **object** |  | [optional] 
+**shots_requested** | **int** |  | [optional] 
+**shots_done** | **int** |  | [optional] 
+**results** | **object** |  | [optional] 
 **metadata_id** | **int** |  | 
 **run_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/ResultIn.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeType.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# ResultIn
+# RuntimeType
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**number_of_qubits** | **int** |  | 
-**execution_time_in_seconds** | **float** |  | 
-**raw_text** | **str** |  | 
-**raw_data** | **object** |  | [optional] 
-**histogram** | **object** |  | [optional] 
-**measurement_mask** | **object** |  | [optional] 
-**quantum_states** | **object** |  | [optional] 
-**measurement_register** | **object** |  | [optional] 
-**metadata_id** | **int** |  | 
-**run_id** | **int** |  | 
+**id** | **int** |  | 
+**name** | **str** |  | 
+**infrastructure** | **str** |  | 
+**description** | **str** |  | 
+**image_id** | **str** |  | 
+**is_hardware** | **bool** |  | 
+**features** | **object** |  | [optional] 
+**default_compiler_config** | **object** |  | [optional] 
+**native_gateset** | **object** |  | [optional] 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Run.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Run.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/RunIn.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/RunIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Runtime.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Runtime.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,13 +5,12 @@
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **id** | **int** |  | 
 **name** | **str** |  | 
 **location** | **str** |  | 
 **status** | [**RuntimeStatus**](RuntimeStatus.md) | OFFLINE: offline&lt;br/&gt;IDLE: idle&lt;br/&gt;EXECUTING: executing&lt;br/&gt;CALIBRATING: calibrating | 
 **last_heartbeat** | **datetime** |  | 
-**authentication_hash** | **str** |  | 
 **runtime_type_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeApi.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/RuntimeTypesApi.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,66 +1,77 @@
-# compute_api_client.RuntimeApi
+# compute_api_client.RuntimeTypesApi
 
 All URIs are relative to *http://localhost*
 
 Method | HTTP request | Description
 ------------- | ------------- | -------------
-[**read_runtime_runtimes_id_get**](RuntimeApi.md#read_runtime_runtimes_id_get) | **GET** /runtimes/{id} | Retrieve runtime
-[**read_runtimes_runtimes_get**](RuntimeApi.md#read_runtimes_runtimes_get) | **GET** /runtimes | List runtimes
+[**read_runtime_type_runtime_types_id_get**](RuntimeTypesApi.md#read_runtime_type_runtime_types_id_get) | **GET** /runtime_types/{id} | Retrieve runtime type
+[**read_runtime_types_runtime_types_get**](RuntimeTypesApi.md#read_runtime_types_runtime_types_get) | **GET** /runtime_types/ | List runtime types
 
 
-# **read_runtime_runtimes_id_get**
-> Runtime read_runtime_runtimes_id_get(id)
+# **read_runtime_type_runtime_types_id_get**
+> RuntimeType read_runtime_type_runtime_types_id_get(id)
 
-Retrieve runtime
+Retrieve runtime type
 
-Get runtime by ID.
+Get runtime type by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.RuntimeApi(api_client)
+    api_instance = compute_api_client.RuntimeTypesApi(api_client)
     id = 56 # int | 
 
     try:
-        # Retrieve runtime
-        api_response = api_instance.read_runtime_runtimes_id_get(id)
+        # Retrieve runtime type
+        api_response = api_instance.read_runtime_type_runtime_types_id_get(id)
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling RuntimeApi->read_runtime_runtimes_id_get: %s\n" % e)
+        print("Exception when calling RuntimeTypesApi->read_runtime_type_runtime_types_id_get: %s\n" % e)
 ```
 
 ### Parameters
 
 Name | Type | Description  | Notes
 ------------- | ------------- | ------------- | -------------
  **id** | **int**|  | 
 
 ### Return type
 
-[**Runtime**](Runtime.md)
+[**RuntimeType**](RuntimeType.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -68,59 +79,70 @@
 |-------------|-------------|------------------|
 **200** | Successful Response |  -  |
 **404** | Not Found |  -  |
 **422** | Validation Error |  -  |
 
 [[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
 
-# **read_runtimes_runtimes_get**
-> list[Runtime] read_runtimes_runtimes_get()
+# **read_runtime_types_runtime_types_get**
+> list[RuntimeType] read_runtime_types_runtime_types_get()
 
-List runtimes
+List runtime types
 
-Read runtimes.
+Read runtime types.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
-    api_instance = compute_api_client.RuntimeApi(api_client)
+    api_instance = compute_api_client.RuntimeTypesApi(api_client)
     
     try:
-        # List runtimes
-        api_response = api_instance.read_runtimes_runtimes_get()
+        # List runtime types
+        api_response = api_instance.read_runtime_types_runtime_types_get()
         pprint(api_response)
     except ApiException as e:
-        print("Exception when calling RuntimeApi->read_runtimes_runtimes_get: %s\n" % e)
+        print("Exception when calling RuntimeTypesApi->read_runtime_types_runtime_types_get: %s\n" % e)
 ```
 
 ### Parameters
 This endpoint does not need any parameter.
 
 ### Return type
 
-[**list[Runtime]**](Runtime.md)
+[**list[RuntimeType]**](RuntimeType.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/RuntimeType.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/ResultIn.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# RuntimeType
+# ResultIn
 
 
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
-**id** | **int** |  | 
-**name** | **str** |  | 
-**infrastructure** | **str** |  | 
-**description** | **str** |  | 
-**image_id** | **str** |  | 
-**is_hardware** | **bool** |  | 
-**features** | **object** |  | [optional] 
-**default_compiler_config** | **object** |  | [optional] 
-**native_gateset** | **object** |  | [optional] 
+**number_of_qubits** | **int** |  | 
+**execution_time_in_seconds** | **float** |  | 
+**shots_requested** | **int** |  | [optional] 
+**shots_done** | **int** |  | [optional] 
+**results** | **object** |  | [optional] 
+**metadata_id** | **int** |  | 
+**run_id** | **int** |  | 
 
 [[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/TeamsApi.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/TeamsApi.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,29 +13,40 @@
 
 Retrieve teams
 
 Get team by ID.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.TeamsApi(api_client)
     id = 56 # int | 
 
     try:
         # Retrieve teams
         api_response = api_instance.read_team_teams_id_get(id)
@@ -52,15 +63,15 @@
 
 ### Return type
 
 [**Team**](Team.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
@@ -77,29 +88,40 @@
 
 List teams
 
 Read teams.
 
 ### Example
 
+* Api Key Authentication (user):
 ```python
 from __future__ import print_function
 import time
 import compute_api_client
 from compute_api_client.rest import ApiException
 from pprint import pprint
 # Defining the host is optional and defaults to http://localhost
 # See configuration.py for a list of all supported configuration parameters.
 configuration = compute_api_client.Configuration(
     host = "http://localhost"
 )
 
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
 
 # Enter a context with an instance of the API client
-with compute_api_client.ApiClient() as api_client:
+with compute_api_client.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = compute_api_client.TeamsApi(api_client)
     
     try:
         # List teams
         api_response = api_instance.read_teams_teams_get()
         pprint(api_response)
@@ -112,15 +134,15 @@
 
 ### Return type
 
 [**list[Team]**](Team.md)
 
 ### Authorization
 
-No authorization required
+[user](../README.md#user)
 
 ### HTTP request headers
 
  - **Content-Type**: Not defined
  - **Accept**: application/json
 
 ### HTTP response details
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/Transaction.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/Transaction.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/User.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/User.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/docs/UserIn.md` & `qi_compute_api_client-0.4.0/compute_api_client/docs/UserIn.md`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/exceptions.py` & `qi_compute_api_client-0.4.0/compute_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/__init__.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,14 @@
 from compute_api_client.models.role import Role
 from compute_api_client.models.run import Run
 from compute_api_client.models.run_in import RunIn
 from compute_api_client.models.run_status import RunStatus
 from compute_api_client.models.runtime import Runtime
 from compute_api_client.models.runtime_status import RuntimeStatus
 from compute_api_client.models.runtime_type import RuntimeType
+from compute_api_client.models.runtime_with_authentication import RuntimeWithAuthentication
 from compute_api_client.models.share_type import ShareType
 from compute_api_client.models.team import Team
 from compute_api_client.models.transaction import Transaction
 from compute_api_client.models.user import User
 from compute_api_client.models.user_in import UserIn
 from compute_api_client.models.validation_error import ValidationError
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/algorithm.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/algorithm_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/algorithm_type.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/algorithm_type.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/batch_run.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/batch_run_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/batch_run_status.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/batch_run_status.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/commit.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/commit.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/commit_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/commit_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/compile_stage.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/compile_stage.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/domain.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/domain.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/file.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/file.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/file_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/file_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/final_result.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/final_result.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/final_result_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/final_result_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/http_not_found_error.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/http_not_found_error.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/http_validation_error.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/language.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/language.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/location_inner.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/location_inner.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/member.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/member.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/member_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/member_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/metadata.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/metadata_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/metadata_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/permission.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/permission.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/permission_group.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/permission_group.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/project.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/project.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/project_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/project_patch.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/project_patch.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/reservation.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/reservation.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/reservation_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/reservation_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/result.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/result.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,69 +36,57 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'created_on': 'datetime',
         'id': 'int',
         'number_of_qubits': 'int',
         'execution_time_in_seconds': 'float',
-        'raw_text': 'str',
-        'raw_data': 'object',
-        'histogram': 'object',
-        'measurement_mask': 'object',
-        'quantum_states': 'object',
-        'measurement_register': 'object',
+        'shots_requested': 'int',
+        'shots_done': 'int',
+        'results': 'object',
         'metadata_id': 'int',
         'run_id': 'int'
     }
 
     attribute_map = {
         'created_on': 'created_on',
         'id': 'id',
         'number_of_qubits': 'number_of_qubits',
         'execution_time_in_seconds': 'execution_time_in_seconds',
-        'raw_text': 'raw_text',
-        'raw_data': 'raw_data',
-        'histogram': 'histogram',
-        'measurement_mask': 'measurement_mask',
-        'quantum_states': 'quantum_states',
-        'measurement_register': 'measurement_register',
+        'shots_requested': 'shots_requested',
+        'shots_done': 'shots_done',
+        'results': 'results',
         'metadata_id': 'metadata_id',
         'run_id': 'run_id'
     }
 
-    def __init__(self, created_on=None, id=None, number_of_qubits=None, execution_time_in_seconds=None, raw_text=None, raw_data=None, histogram=None, measurement_mask=None, quantum_states=None, measurement_register=None, metadata_id=None, run_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, created_on=None, id=None, number_of_qubits=None, execution_time_in_seconds=None, shots_requested=None, shots_done=None, results=None, metadata_id=None, run_id=None, local_vars_configuration=None):  # noqa: E501
         """Result - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._created_on = None
         self._id = None
         self._number_of_qubits = None
         self._execution_time_in_seconds = None
-        self._raw_text = None
-        self._raw_data = None
-        self._histogram = None
-        self._measurement_mask = None
-        self._quantum_states = None
-        self._measurement_register = None
+        self._shots_requested = None
+        self._shots_done = None
+        self._results = None
         self._metadata_id = None
         self._run_id = None
         self.discriminator = None
 
         self.created_on = created_on
         self.id = id
         self.number_of_qubits = number_of_qubits
         self.execution_time_in_seconds = execution_time_in_seconds
-        self.raw_text = raw_text
-        self.raw_data = raw_data
-        self.histogram = histogram
-        self.measurement_mask = measurement_mask
-        self.quantum_states = quantum_states
-        self.measurement_register = measurement_register
+        self.shots_requested = shots_requested
+        self.shots_done = shots_done
+        self.results = results
         self.metadata_id = metadata_id
         self.run_id = run_id
 
     @property
     def created_on(self):
         """Gets the created_on of this Result.  # noqa: E501
 
@@ -199,140 +187,87 @@
         """
         if self.local_vars_configuration.client_side_validation and execution_time_in_seconds is None:  # noqa: E501
             raise ValueError("Invalid value for `execution_time_in_seconds`, must not be `None`")  # noqa: E501
 
         self._execution_time_in_seconds = execution_time_in_seconds
 
     @property
-    def raw_text(self):
-        """Gets the raw_text of this Result.  # noqa: E501
+    def shots_requested(self):
+        """Gets the shots_requested of this Result.  # noqa: E501
 
 
-        :return: The raw_text of this Result.  # noqa: E501
-        :rtype: str
-        """
-        return self._raw_text
-
-    @raw_text.setter
-    def raw_text(self, raw_text):
-        """Sets the raw_text of this Result.
-
-
-        :param raw_text: The raw_text of this Result.  # noqa: E501
-        :type raw_text: str
-        """
-        if self.local_vars_configuration.client_side_validation and raw_text is None:  # noqa: E501
-            raise ValueError("Invalid value for `raw_text`, must not be `None`")  # noqa: E501
-
-        self._raw_text = raw_text
-
-    @property
-    def raw_data(self):
-        """Gets the raw_data of this Result.  # noqa: E501
-
-
-        :return: The raw_data of this Result.  # noqa: E501
-        :rtype: object
-        """
-        return self._raw_data
-
-    @raw_data.setter
-    def raw_data(self, raw_data):
-        """Sets the raw_data of this Result.
-
-
-        :param raw_data: The raw_data of this Result.  # noqa: E501
-        :type raw_data: object
-        """
-
-        self._raw_data = raw_data
-
-    @property
-    def histogram(self):
-        """Gets the histogram of this Result.  # noqa: E501
-
-
-        :return: The histogram of this Result.  # noqa: E501
-        :rtype: object
-        """
-        return self._histogram
-
-    @histogram.setter
-    def histogram(self, histogram):
-        """Sets the histogram of this Result.
-
-
-        :param histogram: The histogram of this Result.  # noqa: E501
-        :type histogram: object
-        """
-
-        self._histogram = histogram
-
-    @property
-    def measurement_mask(self):
-        """Gets the measurement_mask of this Result.  # noqa: E501
-
-
-        :return: The measurement_mask of this Result.  # noqa: E501
-        :rtype: object
+        :return: The shots_requested of this Result.  # noqa: E501
+        :rtype: int
         """
-        return self._measurement_mask
+        return self._shots_requested
 
-    @measurement_mask.setter
-    def measurement_mask(self, measurement_mask):
-        """Sets the measurement_mask of this Result.
+    @shots_requested.setter
+    def shots_requested(self, shots_requested):
+        """Sets the shots_requested of this Result.
 
 
-        :param measurement_mask: The measurement_mask of this Result.  # noqa: E501
-        :type measurement_mask: object
+        :param shots_requested: The shots_requested of this Result.  # noqa: E501
+        :type shots_requested: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                shots_requested is not None and shots_requested > 2147483647):  # noqa: E501
+            raise ValueError("Invalid value for `shots_requested`, must be a value less than or equal to `2147483647`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                shots_requested is not None and shots_requested < -2147483648):  # noqa: E501
+            raise ValueError("Invalid value for `shots_requested`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
 
-        self._measurement_mask = measurement_mask
+        self._shots_requested = shots_requested
 
     @property
-    def quantum_states(self):
-        """Gets the quantum_states of this Result.  # noqa: E501
+    def shots_done(self):
+        """Gets the shots_done of this Result.  # noqa: E501
 
 
-        :return: The quantum_states of this Result.  # noqa: E501
-        :rtype: object
+        :return: The shots_done of this Result.  # noqa: E501
+        :rtype: int
         """
-        return self._quantum_states
+        return self._shots_done
 
-    @quantum_states.setter
-    def quantum_states(self, quantum_states):
-        """Sets the quantum_states of this Result.
+    @shots_done.setter
+    def shots_done(self, shots_done):
+        """Sets the shots_done of this Result.
 
 
-        :param quantum_states: The quantum_states of this Result.  # noqa: E501
-        :type quantum_states: object
+        :param shots_done: The shots_done of this Result.  # noqa: E501
+        :type shots_done: int
         """
+        if (self.local_vars_configuration.client_side_validation and
+                shots_done is not None and shots_done > 2147483647):  # noqa: E501
+            raise ValueError("Invalid value for `shots_done`, must be a value less than or equal to `2147483647`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                shots_done is not None and shots_done < -2147483648):  # noqa: E501
+            raise ValueError("Invalid value for `shots_done`, must be a value greater than or equal to `-2147483648`")  # noqa: E501
 
-        self._quantum_states = quantum_states
+        self._shots_done = shots_done
 
     @property
-    def measurement_register(self):
-        """Gets the measurement_register of this Result.  # noqa: E501
+    def results(self):
+        """Gets the results of this Result.  # noqa: E501
 
 
-        :return: The measurement_register of this Result.  # noqa: E501
+        :return: The results of this Result.  # noqa: E501
         :rtype: object
         """
-        return self._measurement_register
+        return self._results
 
-    @measurement_register.setter
-    def measurement_register(self, measurement_register):
-        """Sets the measurement_register of this Result.
+    @results.setter
+    def results(self, results):
+        """Sets the results of this Result.
 
 
-        :param measurement_register: The measurement_register of this Result.  # noqa: E501
-        :type measurement_register: object
+        :param results: The results of this Result.  # noqa: E501
+        :type results: object
         """
 
-        self._measurement_register = measurement_register
+        self._results = results
 
     @property
     def metadata_id(self):
         """Gets the metadata_id of this Result.  # noqa: E501
 
 
         :return: The metadata_id of this Result.  # noqa: E501
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/role.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/role.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/run.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/run.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/run_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/run_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/run_status.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/run_status.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/runtime.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_with_authentication.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from compute_api_client.configuration import Configuration
 
 
-class Runtime(object):
+class RuntimeWithAuthentication(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -52,15 +52,15 @@
         'status': 'status',
         'last_heartbeat': 'last_heartbeat',
         'authentication_hash': 'authentication_hash',
         'runtime_type_id': 'runtime_type_id'
     }
 
     def __init__(self, id=None, name=None, location=None, status=None, last_heartbeat=None, authentication_hash=None, runtime_type_id=None, local_vars_configuration=None):  # noqa: E501
-        """Runtime - a model defined in OpenAPI"""  # noqa: E501
+        """RuntimeWithAuthentication - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._name = None
         self._location = None
@@ -76,28 +76,28 @@
         self.status = status
         self.last_heartbeat = last_heartbeat
         self.authentication_hash = authentication_hash
         self.runtime_type_id = runtime_type_id
 
     @property
     def id(self):
-        """Gets the id of this Runtime.  # noqa: E501
+        """Gets the id of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The id of this Runtime.  # noqa: E501
+        :return: The id of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: int
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Runtime.
+        """Sets the id of this RuntimeWithAuthentication.
 
 
-        :param id: The id of this Runtime.  # noqa: E501
+        :param id: The id of this RuntimeWithAuthentication.  # noqa: E501
         :type id: int
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 id is not None and id > 2147483647):  # noqa: E501
             raise ValueError("Invalid value for `id`, must be a value less than or equal to `2147483647`")  # noqa: E501
@@ -105,157 +105,157 @@
                 id is not None and id < 1):  # noqa: E501
             raise ValueError("Invalid value for `id`, must be a value greater than or equal to `1`")  # noqa: E501
 
         self._id = id
 
     @property
     def name(self):
-        """Gets the name of this Runtime.  # noqa: E501
+        """Gets the name of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The name of this Runtime.  # noqa: E501
+        :return: The name of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this Runtime.
+        """Sets the name of this RuntimeWithAuthentication.
 
 
-        :param name: The name of this Runtime.  # noqa: E501
+        :param name: The name of this RuntimeWithAuthentication.  # noqa: E501
         :type name: str
         """
         if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
             raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 name is not None and len(name) > 32):
             raise ValueError("Invalid value for `name`, length must be less than or equal to `32`")  # noqa: E501
 
         self._name = name
 
     @property
     def location(self):
-        """Gets the location of this Runtime.  # noqa: E501
+        """Gets the location of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The location of this Runtime.  # noqa: E501
+        :return: The location of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: str
         """
         return self._location
 
     @location.setter
     def location(self, location):
-        """Sets the location of this Runtime.
+        """Sets the location of this RuntimeWithAuthentication.
 
 
-        :param location: The location of this Runtime.  # noqa: E501
+        :param location: The location of this RuntimeWithAuthentication.  # noqa: E501
         :type location: str
         """
         if self.local_vars_configuration.client_side_validation and location is None:  # noqa: E501
             raise ValueError("Invalid value for `location`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 location is not None and len(location) > 32):
             raise ValueError("Invalid value for `location`, length must be less than or equal to `32`")  # noqa: E501
 
         self._location = location
 
     @property
     def status(self):
-        """Gets the status of this Runtime.  # noqa: E501
+        """Gets the status of this RuntimeWithAuthentication.  # noqa: E501
 
         OFFLINE: offline<br/>IDLE: idle<br/>EXECUTING: executing<br/>CALIBRATING: calibrating  # noqa: E501
 
-        :return: The status of this Runtime.  # noqa: E501
+        :return: The status of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: RuntimeStatus
         """
         return self._status
 
     @status.setter
     def status(self, status):
-        """Sets the status of this Runtime.
+        """Sets the status of this RuntimeWithAuthentication.
 
         OFFLINE: offline<br/>IDLE: idle<br/>EXECUTING: executing<br/>CALIBRATING: calibrating  # noqa: E501
 
-        :param status: The status of this Runtime.  # noqa: E501
+        :param status: The status of this RuntimeWithAuthentication.  # noqa: E501
         :type status: RuntimeStatus
         """
         if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
             raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 status is not None and len(status) > 11):
             raise ValueError("Invalid value for `status`, length must be less than or equal to `11`")  # noqa: E501
 
         self._status = status
 
     @property
     def last_heartbeat(self):
-        """Gets the last_heartbeat of this Runtime.  # noqa: E501
+        """Gets the last_heartbeat of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The last_heartbeat of this Runtime.  # noqa: E501
+        :return: The last_heartbeat of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: datetime
         """
         return self._last_heartbeat
 
     @last_heartbeat.setter
     def last_heartbeat(self, last_heartbeat):
-        """Sets the last_heartbeat of this Runtime.
+        """Sets the last_heartbeat of this RuntimeWithAuthentication.
 
 
-        :param last_heartbeat: The last_heartbeat of this Runtime.  # noqa: E501
+        :param last_heartbeat: The last_heartbeat of this RuntimeWithAuthentication.  # noqa: E501
         :type last_heartbeat: datetime
         """
         if self.local_vars_configuration.client_side_validation and last_heartbeat is None:  # noqa: E501
             raise ValueError("Invalid value for `last_heartbeat`, must not be `None`")  # noqa: E501
 
         self._last_heartbeat = last_heartbeat
 
     @property
     def authentication_hash(self):
-        """Gets the authentication_hash of this Runtime.  # noqa: E501
+        """Gets the authentication_hash of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The authentication_hash of this Runtime.  # noqa: E501
+        :return: The authentication_hash of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: str
         """
         return self._authentication_hash
 
     @authentication_hash.setter
     def authentication_hash(self, authentication_hash):
-        """Sets the authentication_hash of this Runtime.
+        """Sets the authentication_hash of this RuntimeWithAuthentication.
 
 
-        :param authentication_hash: The authentication_hash of this Runtime.  # noqa: E501
+        :param authentication_hash: The authentication_hash of this RuntimeWithAuthentication.  # noqa: E501
         :type authentication_hash: str
         """
         if self.local_vars_configuration.client_side_validation and authentication_hash is None:  # noqa: E501
             raise ValueError("Invalid value for `authentication_hash`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 authentication_hash is not None and len(authentication_hash) > 32):
             raise ValueError("Invalid value for `authentication_hash`, length must be less than or equal to `32`")  # noqa: E501
 
         self._authentication_hash = authentication_hash
 
     @property
     def runtime_type_id(self):
-        """Gets the runtime_type_id of this Runtime.  # noqa: E501
+        """Gets the runtime_type_id of this RuntimeWithAuthentication.  # noqa: E501
 
 
-        :return: The runtime_type_id of this Runtime.  # noqa: E501
+        :return: The runtime_type_id of this RuntimeWithAuthentication.  # noqa: E501
         :rtype: int
         """
         return self._runtime_type_id
 
     @runtime_type_id.setter
     def runtime_type_id(self, runtime_type_id):
-        """Sets the runtime_type_id of this Runtime.
+        """Sets the runtime_type_id of this RuntimeWithAuthentication.
 
 
-        :param runtime_type_id: The runtime_type_id of this Runtime.  # noqa: E501
+        :param runtime_type_id: The runtime_type_id of this RuntimeWithAuthentication.  # noqa: E501
         :type runtime_type_id: int
         """
         if self.local_vars_configuration.client_side_validation and runtime_type_id is None:  # noqa: E501
             raise ValueError("Invalid value for `runtime_type_id`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 runtime_type_id is not None and runtime_type_id > 2147483647):  # noqa: E501
             raise ValueError("Invalid value for `runtime_type_id`, must be a value less than or equal to `2147483647`")  # noqa: E501
@@ -303,18 +303,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Runtime):
+        if not isinstance(other, RuntimeWithAuthentication):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Runtime):
+        if not isinstance(other, RuntimeWithAuthentication):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/runtime_status.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_status.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/runtime_type.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/runtime_type.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/share_type.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/share_type.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/team.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/team.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/transaction.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/transaction.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/user.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/user.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/user_in.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/user_in.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/models/validation_error.py` & `qi_compute_api_client-0.4.0/compute_api_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/compute_api_client/rest.py` & `qi_compute_api_client-0.4.0/compute_api_client/rest.py`

 * *Files identical despite different names*

### Comparing `qi_compute_api_client-0.1.0/pyproject.toml` & `qi_compute_api_client-0.4.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 [tool.poetry]
 name = "qi-compute-api-client"
-version = "0.1.0"
+version = "0.4.0"
 description = "An API client for the Compute Job Manager of Quantum Inspire."
 license = "Apache-2.0"
 authors = ["Quantum Inspire <support@quantum-inspire.eu>"]
 readme = "README.md"
 repository = "https://github.com/QuTech-Delft/compute-api-client"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License"
 ]
 packages = [
     { include = "compute_api_client" },
 ]
 exclude = ["compute_api_client/test"]
 
 [tool.poetry.dependencies]
 # Should not exceed package python version, so be conservative
+aiohttp = "^3.8.1"
 python = "^3.7"
-urllib3 = "^1.25.3"
 python-dateutil = "^2.8.2"
-aiohttp = "^3.8.1"
+urllib3 = "^1.25.3"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = {extras = ["toml"], version = "^7.2.0"}
-black = "^22.12.0"
-isort = "^5.11.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qi_compute_api_client-0.1.0/setup.py` & `qi_compute_api_client-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,239 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: qi-compute-api-client
+Version: 0.4.0
+Summary: An API client for the Compute Job Manager of Quantum Inspire.
+Home-page: https://github.com/QuTech-Delft/compute-api-client
+License: Apache-2.0
+Author: Quantum Inspire
+Author-email: support@quantum-inspire.eu
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: urllib3 (>=1.25.3,<2.0.0)
+Project-URL: Repository, https://github.com/QuTech-Delft/compute-api-client
+Description-Content-Type: text/markdown
+
+# compute-api-client
+No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+The `compute_api_client` package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
+
+- API version: 0.1.0
+- Package version: 1.0.0
+- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
+
+## Requirements.
+
+Python 2.7 and 3.4+
+
+## Installation & Usage
+
+This python library package is generated without supporting files like setup.py or requirements files
+
+To be able to use it, you will need these dependencies in your own package that uses this library:
+
+* urllib3 >= 1.25.3
+* six >= 1.10
+* python-dateutil
+* aiohttp
+
+## Getting Started
+
+In your own code, to use this library to connect and interact with compute-api-client,
+you can run the following:
+
+```python
+from __future__ import print_function
+
+import time
+import compute_api_client
+from compute_api_client.rest import ApiException
+from pprint import pprint
+
+# Defining the host is optional and defaults to http://localhost
+# See configuration.py for a list of all supported configuration parameters.
+configuration = compute_api_client.Configuration(
+    host = "http://localhost"
+)
+
+# The client must configure the authentication and authorization parameters
+# in accordance with the API server security policy.
+# Examples for each auth method are provided below, use the example that
+# satisfies your auth use case.
+
+# Configure API key authorization: user
+configuration.api_key['user'] = 'YOUR_API_KEY'
+
+# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
+# configuration.api_key_prefix['user'] = 'Bearer'
+
+
+# Enter a context with an instance of the API client
+async with compute_api_client.ApiClient(configuration) as api_client:
+    # Create an instance of the API class
+    api_instance = compute_api_client.AlgorithmsApi(api_client)
+    algorithm_in = compute_api_client.AlgorithmIn() # AlgorithmIn | 
+
+    try:
+        # Create algorithm
+        api_response = await api_instance.create_algorithm_algorithms_post(algorithm_in)
+        pprint(api_response)
+    except ApiException as e:
+        print("Exception when calling AlgorithmsApi->create_algorithm_algorithms_post: %s\n" % e)
+    
+```
+
+## Documentation for API Endpoints
+
+All URIs are relative to *http://localhost*
+
+Class | Method | HTTP request | Description
+------------ | ------------- | ------------- | -------------
+*AlgorithmsApi* | [**create_algorithm_algorithms_post**](compute_api_client/docs/AlgorithmsApi.md#create_algorithm_algorithms_post) | **POST** /algorithms | Create algorithm
+*AlgorithmsApi* | [**delete_algorithm_algorithms_id_delete**](compute_api_client/docs/AlgorithmsApi.md#delete_algorithm_algorithms_id_delete) | **DELETE** /algorithms/{id} | Destroy algorithm
+*AlgorithmsApi* | [**read_algorithm_algorithms_id_get**](compute_api_client/docs/AlgorithmsApi.md#read_algorithm_algorithms_id_get) | **GET** /algorithms/{id} | Retrieve algorithm
+*AlgorithmsApi* | [**read_algorithms_algorithms_get**](compute_api_client/docs/AlgorithmsApi.md#read_algorithms_algorithms_get) | **GET** /algorithms | List algorithms
+*AlgorithmsApi* | [**update_algorithm_algorithms_id_put**](compute_api_client/docs/AlgorithmsApi.md#update_algorithm_algorithms_id_put) | **PUT** /algorithms/{id} | Update algorithm
+*BatchRunsApi* | [**create_batch_run_batch_runs_post**](compute_api_client/docs/BatchRunsApi.md#create_batch_run_batch_runs_post) | **POST** /batch_runs | Create batch run
+*BatchRunsApi* | [**enqueue_batch_run_batch_runs_id_enqueue_patch**](compute_api_client/docs/BatchRunsApi.md#enqueue_batch_run_batch_runs_id_enqueue_patch) | **PATCH** /batch_runs/{id}/enqueue | Enqueue batch run for execution
+*BatchRunsApi* | [**finish_batch_run_batch_runs_id_finish_patch**](compute_api_client/docs/BatchRunsApi.md#finish_batch_run_batch_runs_id_finish_patch) | **PATCH** /batch_runs/{id}/finish | Finish batch run
+*BatchRunsApi* | [**peek_batch_run_batch_runs_peek_patch**](compute_api_client/docs/BatchRunsApi.md#peek_batch_run_batch_runs_peek_patch) | **PATCH** /batch_runs/peek | Peek batch run
+*BatchRunsApi* | [**pop_batch_run_batch_runs_pop_patch**](compute_api_client/docs/BatchRunsApi.md#pop_batch_run_batch_runs_pop_patch) | **PATCH** /batch_runs/pop | Take batch run
+*BatchRunsApi* | [**read_batch_runs_batch_runs_get**](compute_api_client/docs/BatchRunsApi.md#read_batch_runs_batch_runs_get) | **GET** /batch_runs | List batch runs
+*CommitsApi* | [**create_commit_commits_post**](compute_api_client/docs/CommitsApi.md#create_commit_commits_post) | **POST** /commits | Create commit
+*CommitsApi* | [**delete_commit_commits_id_delete**](compute_api_client/docs/CommitsApi.md#delete_commit_commits_id_delete) | **DELETE** /commits/{id} | Destroy commit
+*CommitsApi* | [**read_commit_commits_id_get**](compute_api_client/docs/CommitsApi.md#read_commit_commits_id_get) | **GET** /commits/{id} | Get commit by ID
+*CommitsApi* | [**read_commits_commits_get**](compute_api_client/docs/CommitsApi.md#read_commits_commits_get) | **GET** /commits | List commits
+*FilesApi* | [**create_file_files_post**](compute_api_client/docs/FilesApi.md#create_file_files_post) | **POST** /files | Create file
+*FilesApi* | [**delete_file_files_id_delete**](compute_api_client/docs/FilesApi.md#delete_file_files_id_delete) | **DELETE** /files/{id} | Destroy file
+*FilesApi* | [**read_file_files_id_get**](compute_api_client/docs/FilesApi.md#read_file_files_id_get) | **GET** /files/{id} | Retrieve file
+*FilesApi* | [**read_files_files_get**](compute_api_client/docs/FilesApi.md#read_files_files_get) | **GET** /files | List files
+*FinalResultsApi* | [**create_final_result_final_results_post**](compute_api_client/docs/FinalResultsApi.md#create_final_result_final_results_post) | **POST** /final_results | Create final result
+*FinalResultsApi* | [**read_final_result_by_run_id_final_results_run_run_id_get**](compute_api_client/docs/FinalResultsApi.md#read_final_result_by_run_id_final_results_run_run_id_get) | **GET** /final_results/run/{run_id} | Retrieve final result by run ID
+*FinalResultsApi* | [**read_final_result_final_results_id_get**](compute_api_client/docs/FinalResultsApi.md#read_final_result_final_results_id_get) | **GET** /final_results/{id} | Retrieve final result
+*LanguagesApi* | [**read_language_languages_id_get**](compute_api_client/docs/LanguagesApi.md#read_language_languages_id_get) | **GET** /languages/{id} | Retrieve language
+*LanguagesApi* | [**read_languages_languages_get**](compute_api_client/docs/LanguagesApi.md#read_languages_languages_get) | **GET** /languages | List languages
+*MembersApi* | [**create_member_members_post**](compute_api_client/docs/MembersApi.md#create_member_members_post) | **POST** /members | Create member
+*MembersApi* | [**delete_member_members_id_delete**](compute_api_client/docs/MembersApi.md#delete_member_members_id_delete) | **DELETE** /members/{id} | Destroy member
+*MembersApi* | [**read_member_members_id_get**](compute_api_client/docs/MembersApi.md#read_member_members_id_get) | **GET** /members/{id} | Retrieve member
+*MembersApi* | [**read_members_members_get**](compute_api_client/docs/MembersApi.md#read_members_members_get) | **GET** /members | List members
+*MetadataApi* | [**create_metadata_metadata_post**](compute_api_client/docs/MetadataApi.md#create_metadata_metadata_post) | **POST** /metadata | Create metadata
+*MetadataApi* | [**read_metadata_by_runtime_id_metadata_runtime_runtime_id_get**](compute_api_client/docs/MetadataApi.md#read_metadata_by_runtime_id_metadata_runtime_runtime_id_get) | **GET** /metadata/runtime/{runtime_id} | Retrieve metadata by runtime ID
+*MetadataApi* | [**read_metadata_metadata_id_get**](compute_api_client/docs/MetadataApi.md#read_metadata_metadata_id_get) | **GET** /metadata/{id} | Get metadata by ID
+*PermissionsApi* | [**read_permission_group_permission_groups_id_get**](compute_api_client/docs/PermissionsApi.md#read_permission_group_permission_groups_id_get) | **GET** /permission_groups/{id} | Retrieve permission groups
+*PermissionsApi* | [**read_permission_groups_permission_groups_get**](compute_api_client/docs/PermissionsApi.md#read_permission_groups_permission_groups_get) | **GET** /permission_groups/ | List permission groups
+*PermissionsApi* | [**read_permission_permissions_id_get**](compute_api_client/docs/PermissionsApi.md#read_permission_permissions_id_get) | **GET** /permissions/{id} | Retrieve permissions
+*PermissionsApi* | [**read_permissions_permissions_get**](compute_api_client/docs/PermissionsApi.md#read_permissions_permissions_get) | **GET** /permissions/ | List permissions
+*ProjectsApi* | [**create_project_projects_post**](compute_api_client/docs/ProjectsApi.md#create_project_projects_post) | **POST** /projects | Create project
+*ProjectsApi* | [**delete_project_projects_id_delete**](compute_api_client/docs/ProjectsApi.md#delete_project_projects_id_delete) | **DELETE** /projects/{id} | Destroy project
+*ProjectsApi* | [**partial_update_project_projects_id_patch**](compute_api_client/docs/ProjectsApi.md#partial_update_project_projects_id_patch) | **PATCH** /projects/{id} | Partially update project
+*ProjectsApi* | [**read_project_projects_id_get**](compute_api_client/docs/ProjectsApi.md#read_project_projects_id_get) | **GET** /projects/{id} | Retrieve project
+*ProjectsApi* | [**read_projects_projects_get**](compute_api_client/docs/ProjectsApi.md#read_projects_projects_get) | **GET** /projects | List projects
+*ProjectsApi* | [**update_project_projects_id_put**](compute_api_client/docs/ProjectsApi.md#update_project_projects_id_put) | **PUT** /projects/{id} | Update project
+*ReservationsApi* | [**create_reservation_reservations_post**](compute_api_client/docs/ReservationsApi.md#create_reservation_reservations_post) | **POST** /reservations | Create reservation
+*ReservationsApi* | [**read_reservation_reservations_id_get**](compute_api_client/docs/ReservationsApi.md#read_reservation_reservations_id_get) | **GET** /reservations/{id} | Retrieve reservation
+*ReservationsApi* | [**read_reservations_reservations_get**](compute_api_client/docs/ReservationsApi.md#read_reservations_reservations_get) | **GET** /reservations | List reservations
+*ReservationsApi* | [**terminate_reservation_reservations_id_terminate_patch**](compute_api_client/docs/ReservationsApi.md#terminate_reservation_reservations_id_terminate_patch) | **PATCH** /reservations/{id}/terminate | Terminate reservation
+*ResultsApi* | [**create_result_results_post**](compute_api_client/docs/ResultsApi.md#create_result_results_post) | **POST** /results | Create result
+*ResultsApi* | [**read_result_results_id_get**](compute_api_client/docs/ResultsApi.md#read_result_results_id_get) | **GET** /results/{id} | Retrieve result
+*ResultsApi* | [**read_results_by_run_id_results_run_run_id_get**](compute_api_client/docs/ResultsApi.md#read_results_by_run_id_results_run_run_id_get) | **GET** /results/run/{run_id} | Retrieve result
+*RunsApi* | [**create_run_runs_post**](compute_api_client/docs/RunsApi.md#create_run_runs_post) | **POST** /runs | Create run
+*RunsApi* | [**delete_run_runs_id_delete**](compute_api_client/docs/RunsApi.md#delete_run_runs_id_delete) | **DELETE** /runs/{id} | Destroy run
+*RunsApi* | [**read_run_runs_id_get**](compute_api_client/docs/RunsApi.md#read_run_runs_id_get) | **GET** /runs/{id} | Retrieve run
+*RunsApi* | [**read_runs_runs_get**](compute_api_client/docs/RunsApi.md#read_runs_runs_get) | **GET** /runs | List runs
+*RunsApi* | [**start_run_runs_id_start_patch**](compute_api_client/docs/RunsApi.md#start_run_runs_id_start_patch) | **PATCH** /runs/{id}/start | Start run
+*RuntimeApi* | [**create_runtime_runtimes_post**](compute_api_client/docs/RuntimeApi.md#create_runtime_runtimes_post) | **POST** /runtimes | Create runtime
+*RuntimeApi* | [**read_runtime_runtimes_id_get**](compute_api_client/docs/RuntimeApi.md#read_runtime_runtimes_id_get) | **GET** /runtimes/{id} | Retrieve runtime
+*RuntimeApi* | [**read_runtimes_runtimes_get**](compute_api_client/docs/RuntimeApi.md#read_runtimes_runtimes_get) | **GET** /runtimes | List runtimes
+*RuntimeTypesApi* | [**read_runtime_type_runtime_types_id_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_type_runtime_types_id_get) | **GET** /runtime_types/{id} | Retrieve runtime type
+*RuntimeTypesApi* | [**read_runtime_types_runtime_types_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_types_runtime_types_get) | **GET** /runtime_types/ | List runtime types
+*TeamsApi* | [**read_team_teams_id_get**](compute_api_client/docs/TeamsApi.md#read_team_teams_id_get) | **GET** /teams/{id} | Retrieve teams
+*TeamsApi* | [**read_teams_teams_get**](compute_api_client/docs/TeamsApi.md#read_teams_teams_get) | **GET** /teams/ | List teams
+*TransactionsApi* | [**read_transaction_transactions_id_get**](compute_api_client/docs/TransactionsApi.md#read_transaction_transactions_id_get) | **GET** /transactions/{id} | Retrieve transactions
+*TransactionsApi* | [**read_transactions_transactions_get**](compute_api_client/docs/TransactionsApi.md#read_transactions_transactions_get) | **GET** /transactions/ | List transactions
+*UsersApi* | [**create_user_users_post**](compute_api_client/docs/UsersApi.md#create_user_users_post) | **POST** /users | Create user
+*UsersApi* | [**delete_user_users_id_delete**](compute_api_client/docs/UsersApi.md#delete_user_users_id_delete) | **DELETE** /users/{id} | Destroy user
+*UsersApi* | [**read_user_users_id_get**](compute_api_client/docs/UsersApi.md#read_user_users_id_get) | **GET** /users/{id} | Retrieve user
+*UsersApi* | [**read_users_users_get**](compute_api_client/docs/UsersApi.md#read_users_users_get) | **GET** /users | List users
+
+
+## Documentation For Models
+
+ - [Algorithm](compute_api_client/docs/Algorithm.md)
+ - [AlgorithmIn](compute_api_client/docs/AlgorithmIn.md)
+ - [AlgorithmType](compute_api_client/docs/AlgorithmType.md)
+ - [BatchRun](compute_api_client/docs/BatchRun.md)
+ - [BatchRunIn](compute_api_client/docs/BatchRunIn.md)
+ - [BatchRunStatus](compute_api_client/docs/BatchRunStatus.md)
+ - [Commit](compute_api_client/docs/Commit.md)
+ - [CommitIn](compute_api_client/docs/CommitIn.md)
+ - [CompileStage](compute_api_client/docs/CompileStage.md)
+ - [Domain](compute_api_client/docs/Domain.md)
+ - [File](compute_api_client/docs/File.md)
+ - [FileIn](compute_api_client/docs/FileIn.md)
+ - [FinalResult](compute_api_client/docs/FinalResult.md)
+ - [FinalResultIn](compute_api_client/docs/FinalResultIn.md)
+ - [HTTPNotFoundError](compute_api_client/docs/HTTPNotFoundError.md)
+ - [HTTPValidationError](compute_api_client/docs/HTTPValidationError.md)
+ - [Language](compute_api_client/docs/Language.md)
+ - [LocationInner](compute_api_client/docs/LocationInner.md)
+ - [Member](compute_api_client/docs/Member.md)
+ - [MemberIn](compute_api_client/docs/MemberIn.md)
+ - [Metadata](compute_api_client/docs/Metadata.md)
+ - [MetadataIn](compute_api_client/docs/MetadataIn.md)
+ - [Permission](compute_api_client/docs/Permission.md)
+ - [PermissionGroup](compute_api_client/docs/PermissionGroup.md)
+ - [Project](compute_api_client/docs/Project.md)
+ - [ProjectIn](compute_api_client/docs/ProjectIn.md)
+ - [ProjectPatch](compute_api_client/docs/ProjectPatch.md)
+ - [Reservation](compute_api_client/docs/Reservation.md)
+ - [ReservationIn](compute_api_client/docs/ReservationIn.md)
+ - [Result](compute_api_client/docs/Result.md)
+ - [ResultIn](compute_api_client/docs/ResultIn.md)
+ - [Role](compute_api_client/docs/Role.md)
+ - [Run](compute_api_client/docs/Run.md)
+ - [RunIn](compute_api_client/docs/RunIn.md)
+ - [RunStatus](compute_api_client/docs/RunStatus.md)
+ - [Runtime](compute_api_client/docs/Runtime.md)
+ - [RuntimeStatus](compute_api_client/docs/RuntimeStatus.md)
+ - [RuntimeType](compute_api_client/docs/RuntimeType.md)
+ - [RuntimeWithAuthentication](compute_api_client/docs/RuntimeWithAuthentication.md)
+ - [ShareType](compute_api_client/docs/ShareType.md)
+ - [Team](compute_api_client/docs/Team.md)
+ - [Transaction](compute_api_client/docs/Transaction.md)
+ - [User](compute_api_client/docs/User.md)
+ - [UserIn](compute_api_client/docs/UserIn.md)
+ - [ValidationError](compute_api_client/docs/ValidationError.md)
+
+
+## Documentation For Authorization
+
+
+## user
+
+- **Type**: API key
+- **API key parameter name**: X-userid
+- **Location**: HTTP header
+
+
+## runtime
+
+- **Type**: API key
+- **API key parameter name**: Authorization
+- **Location**: HTTP header
+
+
+## Author
 
-packages = \
-['compute_api_client', 'compute_api_client.api', 'compute_api_client.models']
 
-package_data = \
-{'': ['*'], 'compute_api_client': ['docs/*']}
 
-install_requires = \
-['aiohttp>=3.8.1,<4.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'urllib3>=1.25.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'qi-compute-api-client',
-    'version': '0.1.0',
-    'description': 'An API client for the Compute Job Manager of Quantum Inspire.',
-    'long_description': '# compute-api-client\nNo description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)\n\nThe `compute_api_client` package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:\n\n- API version: 0.1.0\n- Package version: 1.0.0\n- Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen\n\n## Requirements.\n\nPython 2.7 and 3.4+\n\n## Installation & Usage\n\nThis python library package is generated without supporting files like setup.py or requirements files\n\nTo be able to use it, you will need these dependencies in your own package that uses this library:\n\n* urllib3 >= 1.25.3\n* six >= 1.10\n* python-dateutil\n* aiohttp\n\n## Getting Started\n\nIn your own code, to use this library to connect and interact with compute-api-client,\nyou can run the following:\n\n```python\nfrom __future__ import print_function\n\nimport time\nimport compute_api_client\nfrom compute_api_client.rest import ApiException\nfrom pprint import pprint\n\n# Defining the host is optional and defaults to http://localhost\n# See configuration.py for a list of all supported configuration parameters.\nconfiguration = compute_api_client.Configuration(\n    host = "http://localhost"\n)\n\n\n\n# Enter a context with an instance of the API client\nwith compute_api_client.ApiClient(configuration) as api_client:\n    # Create an instance of the API class\n    api_instance = compute_api_client.AlgorithmsApi(api_client)\n    algorithm_in = compute_api_client.AlgorithmIn() # AlgorithmIn | \n\n    try:\n        # Create algorithm\n        api_response = api_instance.create_algorithm_algorithms_post(algorithm_in)\n        pprint(api_response)\n    except ApiException as e:\n        print("Exception when calling AlgorithmsApi->create_algorithm_algorithms_post: %s\\n" % e)\n    \n```\n\n## Documentation for API Endpoints\n\nAll URIs are relative to *http://localhost*\n\nClass | Method | HTTP request | Description\n------------ | ------------- | ------------- | -------------\n*AlgorithmsApi* | [**create_algorithm_algorithms_post**](compute_api_client/docs/AlgorithmsApi.md#create_algorithm_algorithms_post) | **POST** /algorithms | Create algorithm\n*AlgorithmsApi* | [**delete_algorithm_algorithms_id_delete**](compute_api_client/docs/AlgorithmsApi.md#delete_algorithm_algorithms_id_delete) | **DELETE** /algorithms/{id} | Destroy algorithm\n*AlgorithmsApi* | [**read_algorithm_algorithms_id_get**](compute_api_client/docs/AlgorithmsApi.md#read_algorithm_algorithms_id_get) | **GET** /algorithms/{id} | Retrieve algorithm\n*AlgorithmsApi* | [**read_algorithms_algorithms_get**](compute_api_client/docs/AlgorithmsApi.md#read_algorithms_algorithms_get) | **GET** /algorithms | List algorithms\n*AlgorithmsApi* | [**update_algorithm_algorithms_id_put**](compute_api_client/docs/AlgorithmsApi.md#update_algorithm_algorithms_id_put) | **PUT** /algorithms/{id} | Update algorithm\n*BatchRunsApi* | [**create_batch_run_batch_runs_post**](compute_api_client/docs/BatchRunsApi.md#create_batch_run_batch_runs_post) | **POST** /batch_runs | Create batch run\n*BatchRunsApi* | [**enqueue_batch_run_batch_runs_id_enqueue_patch**](compute_api_client/docs/BatchRunsApi.md#enqueue_batch_run_batch_runs_id_enqueue_patch) | **PATCH** /batch_runs/{id}/enqueue | Enqueue batch run for execution\n*BatchRunsApi* | [**finish_batch_run_batch_runs_id_finish_patch**](compute_api_client/docs/BatchRunsApi.md#finish_batch_run_batch_runs_id_finish_patch) | **PATCH** /batch_runs/{id}/finish | Finish batch run\n*BatchRunsApi* | [**peek_batch_run_batch_runs_peek_patch**](compute_api_client/docs/BatchRunsApi.md#peek_batch_run_batch_runs_peek_patch) | **PATCH** /batch_runs/peek | Peek batch run\n*BatchRunsApi* | [**pop_batch_run_batch_runs_pop_patch**](compute_api_client/docs/BatchRunsApi.md#pop_batch_run_batch_runs_pop_patch) | **PATCH** /batch_runs/pop | Take batch run\n*BatchRunsApi* | [**read_batch_runs_batch_runs_get**](compute_api_client/docs/BatchRunsApi.md#read_batch_runs_batch_runs_get) | **GET** /batch_runs | List batch runs\n*CommitsApi* | [**create_commit_commits_post**](compute_api_client/docs/CommitsApi.md#create_commit_commits_post) | **POST** /commits | Create commit\n*CommitsApi* | [**delete_commit_commits_id_delete**](compute_api_client/docs/CommitsApi.md#delete_commit_commits_id_delete) | **DELETE** /commits/{id} | Destroy commit\n*CommitsApi* | [**read_commit_commits_id_get**](compute_api_client/docs/CommitsApi.md#read_commit_commits_id_get) | **GET** /commits/{id} | Get commit by ID\n*CommitsApi* | [**read_commits_commits_get**](compute_api_client/docs/CommitsApi.md#read_commits_commits_get) | **GET** /commits | List commits\n*FilesApi* | [**create_file_files_post**](compute_api_client/docs/FilesApi.md#create_file_files_post) | **POST** /files | Create file\n*FilesApi* | [**delete_file_files_id_delete**](compute_api_client/docs/FilesApi.md#delete_file_files_id_delete) | **DELETE** /files/{id} | Destroy file\n*FilesApi* | [**read_file_files_id_get**](compute_api_client/docs/FilesApi.md#read_file_files_id_get) | **GET** /files/{id} | Retrieve file\n*FilesApi* | [**read_files_files_get**](compute_api_client/docs/FilesApi.md#read_files_files_get) | **GET** /files | List files\n*FinalResultsApi* | [**create_final_result_final_results_post**](compute_api_client/docs/FinalResultsApi.md#create_final_result_final_results_post) | **POST** /final_results | Create final result\n*FinalResultsApi* | [**read_final_result_by_run_id_final_results_run_run_id_get**](compute_api_client/docs/FinalResultsApi.md#read_final_result_by_run_id_final_results_run_run_id_get) | **GET** /final_results/run/{run_id} | Retrieve final result by run ID\n*FinalResultsApi* | [**read_final_result_final_results_id_get**](compute_api_client/docs/FinalResultsApi.md#read_final_result_final_results_id_get) | **GET** /final_results/{id} | Retrieve final result\n*LanguagesApi* | [**read_language_languages_id_get**](compute_api_client/docs/LanguagesApi.md#read_language_languages_id_get) | **GET** /languages/{id} | Retrieve language\n*LanguagesApi* | [**read_languages_languages_get**](compute_api_client/docs/LanguagesApi.md#read_languages_languages_get) | **GET** /languages | List languages\n*MembersApi* | [**create_member_members_post**](compute_api_client/docs/MembersApi.md#create_member_members_post) | **POST** /members | Create member\n*MembersApi* | [**delete_member_members_id_delete**](compute_api_client/docs/MembersApi.md#delete_member_members_id_delete) | **DELETE** /members/{id} | Destroy member\n*MembersApi* | [**read_member_members_id_get**](compute_api_client/docs/MembersApi.md#read_member_members_id_get) | **GET** /members/{id} | Retrieve member\n*MembersApi* | [**read_members_members_get**](compute_api_client/docs/MembersApi.md#read_members_members_get) | **GET** /members | List members\n*MetadataApi* | [**create_metadata_metadata_post**](compute_api_client/docs/MetadataApi.md#create_metadata_metadata_post) | **POST** /metadata | Create metadata\n*MetadataApi* | [**read_metadata_by_runtime_id_metadata_runtime_runtime_id_get**](compute_api_client/docs/MetadataApi.md#read_metadata_by_runtime_id_metadata_runtime_runtime_id_get) | **GET** /metadata/runtime/{runtime_id} | Retrieve metadata by runtime ID\n*MetadataApi* | [**read_metadata_metadata_id_get**](compute_api_client/docs/MetadataApi.md#read_metadata_metadata_id_get) | **GET** /metadata/{id} | Get metadata by ID\n*PermissionsApi* | [**read_permission_group_permission_groups_id_get**](compute_api_client/docs/PermissionsApi.md#read_permission_group_permission_groups_id_get) | **GET** /permission_groups/{id} | Retrieve permission groups\n*PermissionsApi* | [**read_permission_groups_permission_groups_get**](compute_api_client/docs/PermissionsApi.md#read_permission_groups_permission_groups_get) | **GET** /permission_groups/ | List permission groups\n*PermissionsApi* | [**read_permission_permissions_id_get**](compute_api_client/docs/PermissionsApi.md#read_permission_permissions_id_get) | **GET** /permissions/{id} | Retrieve permissions\n*PermissionsApi* | [**read_permissions_permissions_get**](compute_api_client/docs/PermissionsApi.md#read_permissions_permissions_get) | **GET** /permissions/ | List permissions\n*ProjectsApi* | [**create_project_projects_post**](compute_api_client/docs/ProjectsApi.md#create_project_projects_post) | **POST** /projects | Create project\n*ProjectsApi* | [**delete_project_projects_id_delete**](compute_api_client/docs/ProjectsApi.md#delete_project_projects_id_delete) | **DELETE** /projects/{id} | Destroy project\n*ProjectsApi* | [**partial_update_project_projects_id_patch**](compute_api_client/docs/ProjectsApi.md#partial_update_project_projects_id_patch) | **PATCH** /projects/{id} | Partially update project\n*ProjectsApi* | [**read_project_projects_id_get**](compute_api_client/docs/ProjectsApi.md#read_project_projects_id_get) | **GET** /projects/{id} | Retrieve project\n*ProjectsApi* | [**read_projects_projects_get**](compute_api_client/docs/ProjectsApi.md#read_projects_projects_get) | **GET** /projects | List projects\n*ProjectsApi* | [**update_project_projects_id_put**](compute_api_client/docs/ProjectsApi.md#update_project_projects_id_put) | **PUT** /projects/{id} | Update project\n*ReservationsApi* | [**create_reservation_reservations_post**](compute_api_client/docs/ReservationsApi.md#create_reservation_reservations_post) | **POST** /reservations | Create reservation\n*ReservationsApi* | [**read_reservation_reservations_id_get**](compute_api_client/docs/ReservationsApi.md#read_reservation_reservations_id_get) | **GET** /reservations/{id} | Retrieve reservation\n*ReservationsApi* | [**read_reservations_reservations_get**](compute_api_client/docs/ReservationsApi.md#read_reservations_reservations_get) | **GET** /reservations | List reservations\n*ReservationsApi* | [**terminate_reservation_reservations_id_terminate_patch**](compute_api_client/docs/ReservationsApi.md#terminate_reservation_reservations_id_terminate_patch) | **PATCH** /reservations/{id}/terminate | Terminate reservation\n*ResultsApi* | [**create_result_results_post**](compute_api_client/docs/ResultsApi.md#create_result_results_post) | **POST** /results | Create result\n*ResultsApi* | [**read_result_results_id_get**](compute_api_client/docs/ResultsApi.md#read_result_results_id_get) | **GET** /results/{id} | Retrieve result\n*ResultsApi* | [**read_results_by_run_id_results_run_run_id_get**](compute_api_client/docs/ResultsApi.md#read_results_by_run_id_results_run_run_id_get) | **GET** /results/run/{run_id} | Retrieve result\n*RunsApi* | [**create_run_runs_post**](compute_api_client/docs/RunsApi.md#create_run_runs_post) | **POST** /runs | Create run\n*RunsApi* | [**delete_run_runs_id_delete**](compute_api_client/docs/RunsApi.md#delete_run_runs_id_delete) | **DELETE** /runs/{id} | Destroy run\n*RunsApi* | [**read_run_runs_id_get**](compute_api_client/docs/RunsApi.md#read_run_runs_id_get) | **GET** /runs/{id} | Retrieve run\n*RunsApi* | [**read_runs_runs_get**](compute_api_client/docs/RunsApi.md#read_runs_runs_get) | **GET** /runs | List runs\n*RunsApi* | [**start_run_runs_id_start_patch**](compute_api_client/docs/RunsApi.md#start_run_runs_id_start_patch) | **PATCH** /runs/{id}/start | Start run\n*RuntimeApi* | [**read_runtime_runtimes_id_get**](compute_api_client/docs/RuntimeApi.md#read_runtime_runtimes_id_get) | **GET** /runtimes/{id} | Retrieve runtime\n*RuntimeApi* | [**read_runtimes_runtimes_get**](compute_api_client/docs/RuntimeApi.md#read_runtimes_runtimes_get) | **GET** /runtimes | List runtimes\n*RuntimeTypesApi* | [**read_runtime_type_runtime_types_id_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_type_runtime_types_id_get) | **GET** /runtime_types/{id} | Retrieve runtime type\n*RuntimeTypesApi* | [**read_runtime_types_runtime_types_get**](compute_api_client/docs/RuntimeTypesApi.md#read_runtime_types_runtime_types_get) | **GET** /runtime_types/ | List runtime types\n*TeamsApi* | [**read_team_teams_id_get**](compute_api_client/docs/TeamsApi.md#read_team_teams_id_get) | **GET** /teams/{id} | Retrieve teams\n*TeamsApi* | [**read_teams_teams_get**](compute_api_client/docs/TeamsApi.md#read_teams_teams_get) | **GET** /teams/ | List teams\n*TransactionsApi* | [**read_transaction_transactions_id_get**](compute_api_client/docs/TransactionsApi.md#read_transaction_transactions_id_get) | **GET** /transactions/{id} | Retrieve transactions\n*TransactionsApi* | [**read_transactions_transactions_get**](compute_api_client/docs/TransactionsApi.md#read_transactions_transactions_get) | **GET** /transactions/ | List transactions\n*UsersApi* | [**create_user_users_post**](compute_api_client/docs/UsersApi.md#create_user_users_post) | **POST** /users | Create user\n*UsersApi* | [**delete_user_users_id_delete**](compute_api_client/docs/UsersApi.md#delete_user_users_id_delete) | **DELETE** /users/{id} | Destroy user\n*UsersApi* | [**read_user_users_id_get**](compute_api_client/docs/UsersApi.md#read_user_users_id_get) | **GET** /users/{id} | Retrieve user\n*UsersApi* | [**read_users_users_get**](compute_api_client/docs/UsersApi.md#read_users_users_get) | **GET** /users | List users\n\n\n## Documentation For Models\n\n - [Algorithm](compute_api_client/docs/Algorithm.md)\n - [AlgorithmIn](compute_api_client/docs/AlgorithmIn.md)\n - [AlgorithmType](compute_api_client/docs/AlgorithmType.md)\n - [BatchRun](compute_api_client/docs/BatchRun.md)\n - [BatchRunIn](compute_api_client/docs/BatchRunIn.md)\n - [BatchRunStatus](compute_api_client/docs/BatchRunStatus.md)\n - [Commit](compute_api_client/docs/Commit.md)\n - [CommitIn](compute_api_client/docs/CommitIn.md)\n - [CompileStage](compute_api_client/docs/CompileStage.md)\n - [Domain](compute_api_client/docs/Domain.md)\n - [File](compute_api_client/docs/File.md)\n - [FileIn](compute_api_client/docs/FileIn.md)\n - [FinalResult](compute_api_client/docs/FinalResult.md)\n - [FinalResultIn](compute_api_client/docs/FinalResultIn.md)\n - [HTTPNotFoundError](compute_api_client/docs/HTTPNotFoundError.md)\n - [HTTPValidationError](compute_api_client/docs/HTTPValidationError.md)\n - [Language](compute_api_client/docs/Language.md)\n - [LocationInner](compute_api_client/docs/LocationInner.md)\n - [Member](compute_api_client/docs/Member.md)\n - [MemberIn](compute_api_client/docs/MemberIn.md)\n - [Metadata](compute_api_client/docs/Metadata.md)\n - [MetadataIn](compute_api_client/docs/MetadataIn.md)\n - [Permission](compute_api_client/docs/Permission.md)\n - [PermissionGroup](compute_api_client/docs/PermissionGroup.md)\n - [Project](compute_api_client/docs/Project.md)\n - [ProjectIn](compute_api_client/docs/ProjectIn.md)\n - [ProjectPatch](compute_api_client/docs/ProjectPatch.md)\n - [Reservation](compute_api_client/docs/Reservation.md)\n - [ReservationIn](compute_api_client/docs/ReservationIn.md)\n - [Result](compute_api_client/docs/Result.md)\n - [ResultIn](compute_api_client/docs/ResultIn.md)\n - [Role](compute_api_client/docs/Role.md)\n - [Run](compute_api_client/docs/Run.md)\n - [RunIn](compute_api_client/docs/RunIn.md)\n - [RunStatus](compute_api_client/docs/RunStatus.md)\n - [Runtime](compute_api_client/docs/Runtime.md)\n - [RuntimeStatus](compute_api_client/docs/RuntimeStatus.md)\n - [RuntimeType](compute_api_client/docs/RuntimeType.md)\n - [ShareType](compute_api_client/docs/ShareType.md)\n - [Team](compute_api_client/docs/Team.md)\n - [Transaction](compute_api_client/docs/Transaction.md)\n - [User](compute_api_client/docs/User.md)\n - [UserIn](compute_api_client/docs/UserIn.md)\n - [ValidationError](compute_api_client/docs/ValidationError.md)\n\n\n## Documentation For Authorization\n\n All endpoints do not require authorization.\n\n## Author\n\n\n\n\n',
-    'author': 'Quantum Inspire',
-    'author_email': 'support@quantum-inspire.eu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/QuTech-Delft/compute-api-client',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

