# Comparing `tmp/auto-test-common-1.0.2.tar.gz` & `tmp/auto-test-common-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.0.2.tar", last modified: Wed May 31 02:36:09 2023, max compression
+gzip compressed data, was "auto-test-common-1.0.4.tar", last modified: Thu Jun  1 00:49:05 2023, max compression
```

## Comparing `auto-test-common-1.0.2.tar` & `auto-test-common-1.0.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.650002 auto-test-common-1.0.2/
--rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 02:36:09.650150 auto-test-common-1.0.2/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.617980 auto-test-common-1.0.2/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1505 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       56 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.618414 auto-test-common-1.0.2/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.2/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.620716 auto-test-common-1.0.2/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.2/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.2/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.2/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.623235 auto-test-common-1.0.2/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.2/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.2/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.2/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.624222 auto-test-common-1.0.2/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.2/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.626770 auto-test-common-1.0.2/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.2/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.2/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.2/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.631475 auto-test-common-1.0.2/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.2/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.2/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.637407 auto-test-common-1.0.2/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.2/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11426 2023-05-31 01:20:03.000000 auto-test-common-1.0.2/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.2/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.2/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.638580 auto-test-common-1.0.2/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.642858 auto-test-common-1.0.2/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.2/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.2/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.2/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.2/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.2/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.2/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.649588 auto-test-common-1.0.2/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.2/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.2/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.2/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8348 2023-05-31 02:31:39.000000 auto-test-common-1.0.2/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.2/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.2/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12175 2023-05-29 05:53:50.000000 auto-test-common-1.0.2/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.2/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 auto-test-common-1.0.2/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    17708 2023-05-31 02:35:10.000000 auto-test-common-1.0.2/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2023-05-31 02:36:09.650855 auto-test-common-1.0.2/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1686 2023-05-23 02:48:09.000000 auto-test-common-1.0.2/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.653901 auto-test-common-1.0.4/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-01 00:49:05.654078 auto-test-common-1.0.4/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.634508 auto-test-common-1.0.4/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      547 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1505 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       56 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-06-01 00:49:05.000000 auto-test-common-1.0.4/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.634897 auto-test-common-1.0.4/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.4/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.636244 auto-test-common-1.0.4/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.4/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.4/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.4/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.637543 auto-test-common-1.0.4/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.4/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.4/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.4/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.638183 auto-test-common-1.0.4/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.4/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.639230 auto-test-common-1.0.4/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.4/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.4/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.4/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.641694 auto-test-common-1.0.4/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.4/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.4/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.644734 auto-test-common-1.0.4/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.4/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11473 2023-05-31 08:51:34.000000 auto-test-common-1.0.4/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.4/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.4/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.645588 auto-test-common-1.0.4/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.4/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.4/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.648227 auto-test-common-1.0.4/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.4/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.4/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.4/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.4/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.4/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.4/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-06-01 00:49:05.653385 auto-test-common-1.0.4/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.4/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.4/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.4/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8259 2023-05-31 03:06:08.000000 auto-test-common-1.0.4/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.4/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.4/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12176 2023-05-31 03:06:08.000000 auto-test-common-1.0.4/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.4/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13130 2023-05-31 08:41:08.000000 auto-test-common-1.0.4/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    17708 2023-05-31 02:35:10.000000 auto-test-common-1.0.4/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2023-06-01 00:49:05.654957 auto-test-common-1.0.4/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1784 2023-06-01 00:45:28.000000 auto-test-common-1.0.4/setup.py
```

### Comparing `auto-test-common-1.0.2/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.0.4/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.0.4/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/autotest/base_requests.py` & `auto-test-common-1.0.4/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/autotest/handle_allure.py` & `auto-test-common-1.0.4/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/autotest/handle_assert.py` & `auto-test-common-1.0.4/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/common/api_driver.py` & `auto-test-common-1.0.4/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/common/constant.py` & `auto-test-common-1.0.4/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/common/test.py` & `auto-test-common-1.0.4/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/config/config.py` & `auto-test-common-1.0.4/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/data/data_process.py` & `auto-test-common-1.0.4/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/data/handle_common.py` & `auto-test-common-1.0.4/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/db/handle_db.py` & `auto-test-common-1.0.4/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/db/handle_db_batch.py` & `auto-test-common-1.0.4/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/db/handle_mysqldb.py` & `auto-test-common-1.0.4/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/db/handle_oracle.py` & `auto-test-common-1.0.4/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/db/handle_sqlserver.py` & `auto-test-common-1.0.4/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/file/ReadFile.py` & `auto-test-common-1.0.4/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/file/handle_excel.py` & `auto-test-common-1.0.4/common/file/handle_excel.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             cycleId = get_system_key(Constant.TEST_SRTCYCLE_ID)
             _list = ServicePlatForm.getCaseRun(cycleId, caseNo, casename)
             if _list['status'] == Constant.STATUS_PRE:
                 ServicePlatForm.updateByRunid(_list['caserunid'], Constant.STATUS_AUTOTEST, "")
                 logger.info(f'用例信息:{str(_list)} 添加到执行队列')
                 return True
             else:
-                logger.info(f'用例信息:{str(_list)} 已经被添加到执行队列')
+                logger.info(f' 用例名称:{casename} 用例编号:{caseNo} 用例信息:{str(_list)} 已经被添加到执行队列')
                 return False
         if testdata[Constant.CASE_STATUS].strip() == '否':
             return False
         if DataProcess.isNotNull(get_system_key(Constant.TEST_CASE_NAME_LIST)):
             if testdata[Constant.CASE_TITLE] in eval(get_system_key(Constant.TEST_CASE_NAME_LIST)):
                 return True
             else:
```

### Comparing `auto-test-common-1.0.2/common/file/handle_file.py` & `auto-test-common-1.0.4/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/file/handle_reques.py` & `auto-test-common-1.0.4/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/file/handle_system.py` & `auto-test-common-1.0.4/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/file/handle_yaml.py` & `auto-test-common-1.0.4/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/mq/handle_rabbit.py` & `auto-test-common-1.0.4/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plat/ATF_platform.py` & `auto-test-common-1.0.4/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plat/jenkin_platform.py` & `auto-test-common-1.0.4/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plat/jira_platform.py` & `auto-test-common-1.0.4/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plat/mysql_platform.py` & `auto-test-common-1.0.4/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plat/service_platform.py` & `auto-test-common-1.0.4/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/allure_plugin.py` & `auto-test-common-1.0.4/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/assert_plugin.py` & `auto-test-common-1.0.4/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/atf_plugin.py` & `auto-test-common-1.0.4/common/plugin/atf_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,17 @@
 
 
 
 
 
 
 if __name__ == '__main__':
-    _summary=FilePlugin.load_json("aa.json")
-    print( DataProcess.getDate(int(str(DataPlugin.get_data_jpath(_summary, "$.time.start")).strip()) / 1000))
+    _summary=FilePlugin.load_file("muc.xml")
+    print(_summary)
+
```

### Comparing `auto-test-common-1.0.2/common/plugin/data_bus.py` & `auto-test-common-1.0.4/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/data_plugin.py` & `auto-test-common-1.0.4/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/file_plugin.py` & `auto-test-common-1.0.4/common/plugin/file_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
                     _list = DataPlugin.remove_empty(_list)
                 else:
                     if _replace:
                         _list = DataBus.get_data(_list, _dict, _no_content)
         return _list
 
     @classmethod
-    def load_xml(self, file_name, _xpath,_dict=None, _replace: bool = True, file_path: str = TEST_DATA_PATH, _no_content=0,
+    def load_xml(self, file_name, _xpath, _dict=None, _replace: bool = True, file_path: str = TEST_DATA_PATH, _no_content=0,
                   _remove_null: bool = False):
         """
         把Json模版转换为JSON数据,默认找不到数据用空代替
         :param file_name:
         :param replace:
         :param _dict:
         :param file_path:
```

### Comparing `auto-test-common-1.0.2/common/plugin/hooks_plugin.py` & `auto-test-common-1.0.4/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/common/plugin/pytest_playwright.py` & `auto-test-common-1.0.4/common/plugin/pytest_playwright.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
 
 @pytest.fixture(scope="session")
 def browser_type_launch_args(pytestconfig: Any) -> Dict:
     DataBus.save_init_data()
     launch_options = {}
     headed_option = pytestconfig.getoption("--headed")
-    if DataProcess.isNotNull(get_system_key("headed")):
+    if DataProcess.isNotNull(get_system_key("headed")) and get_system_key("headed") != "NO":
         headed_option = get_system_key("headed")
     if headed_option:
         launch_options["headless"] = False
     elif VSCODE_PYTHON_EXTENSION_ID in sys.argv[0] and _is_debugger_attached():
         # When the VSCode debugger is attached, then launch the browser headed by default
         launch_options["headless"] = False
     browser_channel_option = pytestconfig.getoption("--browser-channel")
```

### Comparing `auto-test-common-1.0.2/common/plugin/pytest_plugin.py` & `auto-test-common-1.0.4/common/plugin/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.2/setup.py` & `auto-test-common-1.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,17 +41,19 @@
         #"opencv-python-headless==4.7.0.72",
         #"ddddocr==1.4.7",
         #"scikit-build==0.17.5",
 
     ],
     entry_points={"pytest11": ["playwright = common.plugin.pytest_playwright"]},
     classifiers=[
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Framework :: Pytest",
     ],
-    python_requires=">=3.8"
+    python_requires=">=3.6"
 )
```

