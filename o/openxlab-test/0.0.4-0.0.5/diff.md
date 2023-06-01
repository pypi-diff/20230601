# Comparing `tmp/openxlab-test-0.0.4.tar.gz` & `tmp/openxlab-test-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-test-0.0.4.tar", last modified: Wed May 31 11:30:51 2023, max compression
+gzip compressed data, was "openxlab-test-0.0.5.tar", last modified: Thu Jun  1 09:13:37 2023, max compression
```

## Comparing `openxlab-test-0.0.4.tar` & `openxlab-test-0.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.638482 openxlab-test-0.0.4/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1523 2023-05-31 11:30:51.638205 openxlab-test-0.0.4/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1115 2023-05-31 11:24:13.000000 openxlab-test-0.0.4/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.610031 openxlab-test-0.0.4/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.4/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.611673 openxlab-test-0.0.4/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.4/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/config/const.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-31 11:30:46.000000 openxlab-test-0.0.4/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.612085 openxlab-test-0.0.4/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.612737 openxlab-test-0.0.4/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.614960 openxlab-test-0.0.4/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     7755 2023-05-30 09:57:52.000000 openxlab-test-0.0.4/openxlab/model/clients/openapi_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/clients/oss_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/clients/upload_service_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.620698 openxlab-test-0.0.4/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1049 2023-05-30 09:23:55.000000 openxlab-test-0.0.4/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.622583 openxlab-test-0.0.4/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-31 09:40:34.000000 openxlab-test-0.0.4/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.627331 openxlab-test-0.0.4/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     5193 2023-05-31 11:30:46.000000 openxlab-test-0.0.4/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-19 05:11:41.000000 openxlab-test-0.0.4/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/update_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/model/handler/upload_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.628195 openxlab-test-0.0.4/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.4/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.4/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.631549 openxlab-test-0.0.4/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.4/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/utils/auth.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/utils/env_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.4/openxlab/utils/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/utils/time_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.632095 openxlab-test-0.0.4/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.632825 openxlab-test-0.0.4/openxlab/xlab/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/clients/auth_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.633545 openxlab-test-0.0.4/openxlab/xlab/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/commands/config_command.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.634208 openxlab-test-0.0.4/openxlab/xlab/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.635537 openxlab-test-0.0.4/openxlab/xlab/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/openxlab/xlab/handler/user_config.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-31 09:40:20.000000 openxlab-test-0.0.4/openxlab/xlab/handler/user_token.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:30:51.637825 openxlab-test-0.0.4/openxlab_test.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1523 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       53 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-31 11:30:51.000000 openxlab-test-0.0.4/openxlab_test.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-19 08:42:18.000000 openxlab-test-0.0.4/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-31 11:30:51.638576 openxlab-test-0.0.4/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1188 2023-05-31 11:05:27.000000 openxlab-test-0.0.4/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.031533 openxlab-test-0.0.5/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1523 2023-06-01 09:13:37.031262 openxlab-test-0.0.5/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1115 2023-05-31 11:24:13.000000 openxlab-test-0.0.5/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:36.999236 openxlab-test-0.0.5/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.5/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.001067 openxlab-test-0.0.5/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.5/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/config/const.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-06-01 08:30:38.000000 openxlab-test-0.0.5/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.001589 openxlab-test-0.0.5/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.002335 openxlab-test-0.0.5/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.004887 openxlab-test-0.0.5/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     7755 2023-05-30 09:57:52.000000 openxlab-test-0.0.5/openxlab/model/clients/openapi_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/clients/oss_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/clients/upload_service_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.011028 openxlab-test-0.0.5/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1049 2023-05-30 09:23:55.000000 openxlab-test-0.0.5/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.013127 openxlab-test-0.0.5/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-31 09:40:34.000000 openxlab-test-0.0.5/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.019024 openxlab-test-0.0.5/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5130 2023-06-01 08:29:08.000000 openxlab-test-0.0.5/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-19 05:11:41.000000 openxlab-test-0.0.5/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/update_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/model/handler/upload_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.019894 openxlab-test-0.0.5/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.5/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.5/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.023128 openxlab-test-0.0.5/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.5/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/utils/auth.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/utils/env_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.5/openxlab/utils/file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/utils/time_util.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.024008 openxlab-test-0.0.5/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.024860 openxlab-test-0.0.5/openxlab/xlab/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/clients/auth_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.025987 openxlab-test-0.0.5/openxlab/xlab/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/commands/config_command.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.026928 openxlab-test-0.0.5/openxlab/xlab/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.028558 openxlab-test-0.0.5/openxlab/xlab/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/openxlab/xlab/handler/user_config.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-31 09:40:20.000000 openxlab-test-0.0.5/openxlab/xlab/handler/user_token.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-06-01 09:13:37.030867 openxlab-test-0.0.5/openxlab_test.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1523 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       53 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-06-01 09:13:36.000000 openxlab-test-0.0.5/openxlab_test.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-19 08:42:18.000000 openxlab-test-0.0.5/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-06-01 09:13:37.031625 openxlab-test-0.0.5/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1188 2023-05-31 11:05:27.000000 openxlab-test-0.0.5/setup.py
```

### Comparing `openxlab-test-0.0.4/PKG-INFO` & `openxlab-test-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab-test
-Version: 0.0.4
+Version: 0.0.5
 Summary: openxlab-test
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-test-0.0.4/README.md` & `openxlab-test-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/cli.py` & `openxlab-test-0.0.5/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/demo_cmd/__init__.py` & `openxlab-test-0.0.5/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/clients/openapi_client.py` & `openxlab-test-0.0.5/openxlab/model/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/clients/oss_client.py` & `openxlab-test-0.0.5/openxlab/model/clients/oss_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/clients/upload_service_client.py` & `openxlab-test-0.0.5/openxlab/model/clients/upload_service_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/__init__.py` & `openxlab-test-0.0.5/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/create.py` & `openxlab-test-0.0.5/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/download.py` & `openxlab-test-0.0.5/openxlab/model/commands/download.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/init.py` & `openxlab-test-0.0.5/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/list.py` & `openxlab-test-0.0.5/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/remove.py` & `openxlab-test-0.0.5/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/upload.py` & `openxlab-test-0.0.5/openxlab/model/commands/upload.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/commands/visibility.py` & `openxlab-test-0.0.5/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/common/constants.py` & `openxlab-test-0.0.5/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/common/meta_file_util.py` & `openxlab-test-0.0.5/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/common/response_dto.py` & `openxlab-test-0.0.5/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/create_repository.py` & `openxlab-test-0.0.5/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/download_file.py` & `openxlab-test-0.0.5/openxlab/model/handler/download_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 
 from openxlab.model.clients.openapi_client import OpenapiClient
 from openxlab.model.common.constants import endpoint, token, default_metafile_template_name, model_cache_path
 
 logger = logging.getLogger("openxlab.model")
 
 
-def download(model_repo, model_name=None, filepath=None, output=None, overwrite=False) -> None:
+def download(model_repo, model_name=None, output=None, overwrite=False) -> None:
     """
     download model file|meta file|log filee|readme file
     usage: cli & sdk
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
         if isinstance(model_name, str):
             model_name = [model_name]
-        if isinstance(filepath, str):
-            filepath = [filepath]
+        filepath = None
         models, files = client.get_download_url(username, repository, model_name, filepath)
 
     except ValueError as e:
         print(f"Error: {e}")
         return
     file_path_download = []
     for i_name, i_model in models.items() if models is not None else []:
```

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/query_repo_model.py` & `openxlab-test-0.0.5/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-test-0.0.5/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/update_repository.py` & `openxlab-test-0.0.5/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/model/handler/upload_file.py` & `openxlab-test-0.0.5/openxlab/model/handler/upload_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/types/command_type.py` & `openxlab-test-0.0.5/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/utils/file.py` & `openxlab-test-0.0.5/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/utils/time_util.py` & `openxlab-test-0.0.5/openxlab/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/xlab/clients/auth_client.py` & `openxlab-test-0.0.5/openxlab/xlab/clients/auth_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/xlab/commands/config_command.py` & `openxlab-test-0.0.5/openxlab/xlab/commands/config_command.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/xlab/common/response_dto.py` & `openxlab-test-0.0.5/openxlab/xlab/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/xlab/handler/user_config.py` & `openxlab-test-0.0.5/openxlab/xlab/handler/user_config.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab/xlab/handler/user_token.py` & `openxlab-test-0.0.5/openxlab/xlab/handler/user_token.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/openxlab_test.egg-info/PKG-INFO` & `openxlab-test-0.0.5/openxlab_test.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openxlab-test
-Version: 0.0.4
+Version: 0.0.5
 Summary: openxlab-test
 Home-page: https://github.com/xxx/xxxx
 Author: Openxlab Contributors
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: openxlab,xxxx
 Platform: UNKNOWN
```

### Comparing `openxlab-test-0.0.4/openxlab_test.egg-info/SOURCES.txt` & `openxlab-test-0.0.5/openxlab_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/pyproject.toml` & `openxlab-test-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.4/setup.py` & `openxlab-test-0.0.5/setup.py`

 * *Files identical despite different names*

