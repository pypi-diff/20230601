# Comparing `tmp/aind_metadata_service-0.4.5.tar.gz` & `tmp/aind_metadata_service-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.5.tar", last modified: Wed May 31 22:58:51 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.6.tar", last modified: Thu Jun  1 21:46:59 2023, max compression
```

## Comparing `aind_metadata_service-0.4.5.tar` & `aind_metadata_service-0.4.6.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.788429 aind_metadata_service-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.736429 aind_metadata_service-0.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.748429 aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.752429 aind_metadata_service-0.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 22:58:51.788429 aind_metadata_service-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.752429 aind_metadata_service-0.4.5/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.752429 aind_metadata_service-0.4.5/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:58:51.788429 aind_metadata_service-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.740429 aind_metadata_service-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.756429 aind_metadata_service-0.4.5/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.760429 aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.760429 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.760429 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.764429 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113119 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.756429 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 22:58:51.000000 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-31 22:58:51.000000 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:58:51.000000 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 22:58:51.000000 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 22:58:51.000000 aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.764429 aind_metadata_service-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.768429 aind_metadata_service-0.4.5/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.740429 aind_metadata_service-0.4.5/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.768429 aind_metadata_service-0.4.5/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/json_responses/mapped_sp_procedure.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.744429 aind_metadata_service-0.4.5/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.744429 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.772429 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.776430 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.744429 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.780429 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.784429 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.784429 aind_metadata_service-0.4.5/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.784429 aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:58:51.788429 aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-05-31 22:58:32.000000 aind_metadata_service-0.4.5/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.378024 aind_metadata_service-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.386024 aind_metadata_service-0.4.6/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.378024 aind_metadata_service-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 21:46:45.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13629 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.394024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113119 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.390024 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:46:59.000000 aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.398024 aind_metadata_service-0.4.6/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12035 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.402024 aind_metadata_service-0.4.6/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.402024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.406024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.382024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.406024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9769 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:46:59.410024 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-01 21:46:44.000000 aind_metadata_service-0.4.6/tests/test_response_handler.py
```

### Comparing `aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.6/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/.github/workflows/ci.yml` & `aind_metadata_service-0.4.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/.github/workflows/publish.yml` & `aind_metadata_service-0.4.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/.gitignore` & `aind_metadata_service-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/Dockerfile` & `aind_metadata_service-0.4.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/LICENSE` & `aind_metadata_service-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/PKG-INFO` & `aind_metadata_service-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.5
+Version: 0.4.6
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.5/README.md` & `aind_metadata_service-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/doc_template/Makefile` & `aind_metadata_service-0.4.6/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/doc_template/make.bat` & `aind_metadata_service-0.4.6/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.6/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/doc_template/source/conf.py` & `aind_metadata_service-0.4.6/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/pyproject.toml` & `aind_metadata_service-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module to create clients to connect to databases."""
+import logging
 from enum import Enum
 from typing import List, Optional
 from xml.etree import ElementTree as ET
 
 import pyodbc
 from aind_data_schema import Procedures, Subject
 from aind_data_schema.procedures import (
@@ -106,15 +107,16 @@
                         subjects
                     )
                     return response
                 else:
                     subject = subjects[0]
                     response = Responses.model_response(subject)
                     return response
-        except pyodbc.Error:
+        except Exception as e:
+            logging.error(repr(e))
             return Responses.internal_server_error_response()
 
     def get_procedures_info(self, subject_id: str) -> JSONResponse:
         """
         Method to retrieve LAS procedures from subject_id (int)
         Parameters
         ----------
@@ -138,15 +140,16 @@
             else:
                 lth = LabTracksResponseHandler()
                 subject_procedures = lth.map_response_to_procedures(results)
                 procedures = Procedures.construct(subject_id=subject_id)
                 procedures.subject_procedures = subject_procedures
                 response = Responses.model_response(procedures)
             return response
-        except pyodbc.Error:
+        except Exception as e:
+            logging.error(repr(e))
             return Responses.internal_server_error_response()
 
 
 class MouseCustomClassFields(Enum):
     """
     LabTracks stores an XML string in the class_values field. We can extract
     the full genotype of the mouse from that field.
```

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/response_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Module to handle responses"""
 import json
+import logging
 from typing import List
 
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from pydantic import BaseModel, validate_model
 
 from aind_metadata_service.client import StatusCodes
@@ -114,81 +115,88 @@
     def combine_procedure_responses(
         lb_response: JSONResponse, sp_response: JSONResponse
     ) -> JSONResponse:
         """
         Combines JSONResponses from Labtracks and Sharepoint clients.
         Handles validation errors and special cases.
         """
-        lb_contents = json.loads(lb_response.body)
-        sp_contents = json.loads(sp_response.body)
-        sp_status_code = sp_response.status_code
-        lb_status_code = lb_response.status_code
-        if sp_status_code == 500 and lb_status_code == 500:
+        try:
+            lb_contents = json.loads(lb_response.body)
+            sp_contents = json.loads(sp_response.body)
+            sp_status_code = sp_response.status_code
+            lb_status_code = lb_response.status_code
+            if sp_status_code == 500 and lb_status_code == 500:
+                return Responses.internal_server_error_response()
+            if sp_status_code == 503 and lb_status_code == 503:
+                return Responses.connection_error_response()
+            if sp_status_code == 404 and lb_status_code == 404:
+                return Responses.no_data_found_response()
+            if sp_status_code < 300 and lb_status_code == 404:
+                return sp_response
+            if sp_status_code == 404 and lb_status_code < 300:
+                return lb_response
+            # handles combination of invalid responses
+            if lb_status_code == 406 and sp_status_code == 406:
+                lb_data = lb_contents["data"]["subject_procedures"]
+                sp_data = sp_contents["data"]["subject_procedures"]
+                combined_data = lb_data + sp_data
+                lb_contents["data"]["subject_procedures"] = combined_data
+                message1 = sp_contents["message"]
+                message2 = lb_contents["message"]
+                return JSONResponse(
+                    status_code=StatusCodes.INVALID_DATA.value,
+                    content=(
+                        {
+                            "message": f"Message 1: {message1}, "
+                            f"Message 2: {message2}",
+                            "data": lb_contents["data"],
+                        }
+                    ),
+                )
+            # handles combinations of valid and invalid responses
+            if (sp_status_code < 300 and lb_status_code == 406) or (
+                lb_status_code < 300 and sp_status_code == 406
+            ):
+                lb_data = lb_contents["data"]["subject_procedures"]
+                sp_data = sp_contents["data"]["subject_procedures"]
+                combined_data = lb_data + sp_data
+                sp_contents["data"]["subject_procedures"] = combined_data
+                return Responses.multi_status_response(
+                    message1=sp_contents["message"],
+                    message2=lb_contents["message"],
+                    data=sp_contents["data"],
+                )
+            # handles case when both responses are valid
+            if sp_status_code < 300 and lb_status_code < 300:
+                lb_data = lb_contents["data"]["subject_procedures"]
+                sp_data = sp_contents["data"]["subject_procedures"]
+                combined_data = lb_data + sp_data
+                lb_contents["data"]["subject_procedures"] = combined_data
+                return JSONResponse(
+                    status_code=StatusCodes.VALID_DATA.value,
+                    content=(
+                        {
+                            "message": "Valid Model.",
+                            "data": lb_contents["data"],
+                        }
+                    ),
+                )
+            # handles combination of server/connection error and valid response
+            if sp_status_code in (500, 503) and lb_status_code < 300:
+                lb_data = lb_contents["data"]["subject_procedures"]
+                lb_contents["data"]["subject_procedures"] = lb_data
+                return Responses.multi_status_response(
+                    message1=sp_contents["message"],
+                    message2=lb_contents["message"],
+                    data=lb_contents["data"],
+                )
+            if sp_status_code < 300 and lb_status_code in (500, 503):
+                sp_data = sp_contents["data"]["subject_procedures"]
+                sp_contents["data"]["subject_procedures"] = sp_data
+                return Responses.multi_status_response(
+                    message1=sp_contents["message"],
+                    message2=lb_contents["message"],
+                    data=sp_contents["data"],
+                )
+        except Exception as e:
+            logging.error(repr(e))
             return Responses.internal_server_error_response()
-        if sp_status_code == 503 and lb_status_code == 503:
-            return Responses.connection_error_response()
-        if sp_status_code == 404 and lb_status_code == 404:
-            return Responses.no_data_found_response()
-        if sp_status_code < 300 and lb_status_code == 404:
-            return sp_response
-        if sp_status_code == 404 and lb_status_code < 300:
-            return lb_response
-        # handles combination of invalid responses
-        if lb_status_code == 406 and sp_status_code == 406:
-            lb_data = lb_contents["data"]["subject_procedures"]
-            sp_data = sp_contents["data"]["subject_procedures"]
-            combined_data = lb_data + sp_data
-            lb_contents["data"]["subject_procedures"] = combined_data
-            message1 = sp_contents["message"]
-            message2 = lb_contents["message"]
-            return JSONResponse(
-                status_code=StatusCodes.INVALID_DATA.value,
-                content=(
-                    {
-                        "message": f"Message 1: {message1}, "
-                        f"Message 2: {message2}",
-                        "data": lb_contents["data"],
-                    }
-                ),
-            )
-        # handles combinations of valid and invalid responses
-        if (sp_status_code < 300 and lb_status_code == 406) or (
-            lb_status_code < 300 and sp_status_code == 406
-        ):
-            lb_data = lb_contents["data"]["subject_procedures"]
-            sp_data = sp_contents["data"]["subject_procedures"]
-            combined_data = lb_data + sp_data
-            sp_contents["data"]["subject_procedures"] = combined_data
-            return Responses.multi_status_response(
-                message1=sp_contents["message"],
-                message2=lb_contents["message"],
-                data=sp_contents["data"],
-            )
-        # handles case when both responses are valid
-        if sp_status_code < 300 and lb_status_code < 300:
-            lb_data = lb_contents["data"]["subject_procedures"]
-            sp_data = sp_contents["data"]["subject_procedures"]
-            combined_data = lb_data + sp_data
-            lb_contents["data"]["subject_procedures"] = combined_data
-            return JSONResponse(
-                status_code=StatusCodes.VALID_DATA.value,
-                content=(
-                    {"message": "Valid Model.", "data": lb_contents["data"]}
-                ),
-            )
-        # handles combination of server/connection error and valid response
-        if sp_status_code in (500, 503) and lb_status_code < 300:
-            lb_data = lb_contents["data"]["subject_procedures"]
-            lb_contents["data"]["subject_procedures"] = lb_data
-            return Responses.multi_status_response(
-                message1=sp_contents["message"],
-                message2=lb_contents["message"],
-                data=lb_contents["data"],
-            )
-        if sp_status_code < 300 and lb_status_code in (500, 503):
-            sp_data = sp_contents["data"]["subject_procedures"]
-            sp_contents["data"]["subject_procedures"] = sp_data
-            return Responses.multi_status_response(
-                message1=sp_contents["message"],
-                message2=lb_contents["message"],
-                data=sp_contents["data"],
-            )
```

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Module to create client to connect to sharepoint database"""
 
+import logging
+
 from aind_data_schema.procedures import Procedures
 from fastapi.responses import JSONResponse
 from office365.runtime.auth.client_credential import ClientCredential
 from office365.sharepoint.client_context import ClientContext
 
 from aind_metadata_service.response_handler import Responses
 from aind_metadata_service.sharepoint.nsb2019.procedures import (
@@ -59,35 +61,38 @@
 
         Returns
         -------
         JSONResponse
           A response
 
         """
-        # TODO: Add try to handle internal server error response.
-        subject_procedures = []
-        nsb_ctx = self.nsb_client_context
-        nsb_2019_mapper = NSB2019Procedures()
-        nsb_2023_mapper = NSB2023Procedures()
-        procedures2019 = nsb_2019_mapper.get_procedures_from_sharepoint(
-            subject_id=subject_id,
-            client_context=nsb_ctx,
-            list_title=self.nsb_list_title_2019,
-        )
-        procedures2023 = nsb_2023_mapper.get_procedures_from_sharepoint(
-            subject_id=subject_id,
-            client_context=nsb_ctx,
-            list_title=self.nsb_list_title_2023,
-        )
-        subject_procedures.extend(procedures2019)
-        subject_procedures.extend(procedures2023)
-        response = self._handle_response_from_sharepoint(
-            subject_id=subject_id, subject_procedures=subject_procedures
-        )
-        return response
+        try:
+            subject_procedures = []
+            nsb_ctx = self.nsb_client_context
+            nsb_2019_mapper = NSB2019Procedures()
+            nsb_2023_mapper = NSB2023Procedures()
+            procedures2019 = nsb_2019_mapper.get_procedures_from_sharepoint(
+                subject_id=subject_id,
+                client_context=nsb_ctx,
+                list_title=self.nsb_list_title_2019,
+            )
+            procedures2023 = nsb_2023_mapper.get_procedures_from_sharepoint(
+                subject_id=subject_id,
+                client_context=nsb_ctx,
+                list_title=self.nsb_list_title_2023,
+            )
+            subject_procedures.extend(procedures2019)
+            subject_procedures.extend(procedures2023)
+            response = self._handle_response_from_sharepoint(
+                subject_id=subject_id, subject_procedures=subject_procedures
+            )
+            return response
+        except Exception as e:
+            logging.error(repr(e))
+            return Responses.internal_server_error_response()
 
     @staticmethod
     def _handle_response_from_sharepoint(
         subject_id: str, subject_procedures=None
     ) -> JSONResponse:
         """
         Maps the response from SharePoint into a Procedures model
```

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/mapping.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/models.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service/sharepoint/nsb2023/procedures.py` & `aind_metadata_service-0.4.6/src/aind_metadata_service/sharepoint/nsb2023/procedures.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.5
+Version: 0.4.6
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.5/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.6/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 src/aind_metadata_service/sharepoint/nsb2019/procedures.py
 src/aind_metadata_service/sharepoint/nsb2023/__init__.py
 src/aind_metadata_service/sharepoint/nsb2023/mapping.py
 src/aind_metadata_service/sharepoint/nsb2023/models.py
 src/aind_metadata_service/sharepoint/nsb2023/procedures.py
 tests/__init__.py
 tests/test_client.py
-tests/test_response_handle.py
+tests/test_response_handler.py
 tests/labtracks/__init__.py
 tests/labtracks/test_client.py
 tests/labtracks/test_query_builder.py
 tests/labtracks/test_response_handler.py
 tests/resources/json_responses/combined.json
 tests/resources/json_responses/mapped_las_procedure.json
 tests/resources/json_responses/mapped_sp_procedure.json
```

### Comparing `aind_metadata_service-0.4.5/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.6/tests/labtracks/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Module to test LabTracks Client methods"""
 
 import datetime
 import decimal
 import unittest
-from unittest.mock import Mock, patch
+from unittest.mock import MagicMock, Mock, call, patch
 
 import pyodbc
 from aind_data_schema.subject import Sex
 
 from aind_metadata_service.labtracks.client import LabTracksClient
 from aind_metadata_service.response_handler import Responses
-
-from .test_response_handler import TestResponseExamples
+from tests.labtracks.test_response_handler import TestResponseExamples
 
 
 class TestLabTracksClient(unittest.TestCase):
     """Tests client methods"""
 
     driver = "{FreeTDS}"
     server = "0.0.0.0"
@@ -44,21 +43,24 @@
         )
 
         self.assertEqual(
             self.lb_client.connection_str, expected_connection_string
         )
 
     @patch("pyodbc.connect")
+    @patch("logging.error")
     def test_labtracks_client_internal_server_error(
-        self, mock_connect: Mock
+        self, mock_log: MagicMock, mock_connect: Mock
     ) -> None:
         """
         Tests that pyodbc errors are returned to client properly
         Parameters
         ----------
+        mock_log : MagicMock
+            Mock the logging error.
         mock_connect : Mock
             A mocked Connection class that can be used to override methods
             without connecting to sqlserver
 
         Returns
         -------
             pass
@@ -70,14 +72,17 @@
 
         type(mock_connect.return_value).cursor = mock_cursor
 
         response1 = self.lb_client.get_subject_info("123")
         response2 = self.lb_client.get_procedures_info("123")
         expected_response = Responses.internal_server_error_response()
         mock_connect.assert_called()
+        mock_log.assert_has_calls(
+            [call("ProgrammingError()"), call("ProgrammingError()")]
+        )
         self.assertEqual(response1.status_code, expected_response.status_code)
         self.assertEqual(response1.body, expected_response.body)
         self.assertEqual(response2.status_code, expected_response.status_code)
         self.assertEqual(response2.body, expected_response.body)
 
     @patch("pyodbc.connect")
     def test_id_does_not_exist(self, _) -> None:
```

### Comparing `aind_metadata_service-0.4.5/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.6/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.6/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.4.6/tests/resources/json_responses/combined.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.4.6/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.6/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.6/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/sharepoint/nsb2023/test_models.py` & `aind_metadata_service-0.4.6/tests/sharepoint/nsb2023/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.6/tests/sharepoint/test_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 import json
 import logging
 import os
 import unittest
 from pathlib import Path
 from typing import List, Tuple
-from unittest.mock import MagicMock, patch
+from unittest.mock import MagicMock, Mock, patch
 
+from aind_metadata_service.response_handler import Responses
 from aind_metadata_service.sharepoint.client import SharePointClient
 
 if os.getenv("LOG_LEVEL"):  # pragma: no cover
     logging.basicConfig(level=os.getenv("LOG_LEVEL"))
 
 TEST_DIR = Path(os.path.dirname(os.path.realpath(__file__))) / ".."
 DIR_RAW_2019 = TEST_DIR / "resources" / "sharepoint" / "nsb2019" / "raw"
@@ -127,10 +128,41 @@
         expected_subject_procedures.sort(key=lambda x: str(x))
         contents["data"]["subject_procedures"].sort(key=lambda x: str(x))
         self.assertEqual(200, response.status_code)
         self.assertEqual(
             expected_subject_procedures, contents["data"]["subject_procedures"]
         )
 
+    @patch("aind_metadata_service.sharepoint.client.ClientContext")
+    @patch(
+        "aind_metadata_service.sharepoint.nsb2023.procedures."
+        "NSB2023Procedures.get_procedures_from_sharepoint"
+    )
+    @patch("logging.error")
+    def test_error_response(
+        self,
+        mock_log: MagicMock,
+        mock_error: MagicMock,
+        mock_sharepoint_client: MagicMock,
+    ):
+        """Tests internal server error response caught correctly."""
+
+        client = SharePointClient(
+            nsb_site_url="some_url",
+            nsb_list_title_2019="some_list_title2019",
+            nsb_list_title_2023="some_list_title2023",
+            client_id="some_client_id",
+            client_secret="some_client_secret",
+        )
+
+        mock_error.side_effect = Mock(side_effect=BrokenPipeError)
+
+        response = client.get_procedure_info("12345")
+        expected_response = Responses.internal_server_error_response()
+        mock_sharepoint_client.assert_called_once()
+        mock_log.assert_called_once_with("BrokenPipeError()")
+        self.assertEqual(500, expected_response.status_code)
+        self.assertEqual(response.body, expected_response.body)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aind_metadata_service-0.4.5/tests/test_client.py` & `aind_metadata_service-0.4.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.5/tests/test_response_handle.py` & `aind_metadata_service-0.4.6/tests/test_response_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """"Tests response_handler module"""
 
 import json
 import os
 import unittest
 from pathlib import Path
+from unittest.mock import MagicMock, Mock, patch
 
 from aind_data_schema.procedures import Procedures
 from aind_data_schema.subject import Species, Subject
 from fastapi.encoders import jsonable_encoder
 from fastapi.responses import JSONResponse
 from pydantic import validate_model
 
@@ -256,10 +257,29 @@
             ),
         )
         self.assertEqual(combined_response_2.body, expected_response_2.body)
         self.assertEqual(
             combined_response_2.status_code, expected_response_2.status_code
         )
 
+    @patch("json.loads")
+    @patch("logging.error")
+    def test_error_combined_response(
+        self, mock_log: MagicMock, mock_json_error: MagicMock
+    ):
+        """Tests internal server error caught and logged correctly."""
+        response1 = JSONResponse(las_subject_procedures)
+        response2 = JSONResponse(sp_subject_procedures)
+
+        mock_json_error.side_effect = Mock(side_effect=KeyError)
+
+        response = Responses.combine_procedure_responses(
+            lb_response=response1, sp_response=response2
+        )
+        expected_response = Responses.internal_server_error_response()
+        mock_log.assert_called_once_with("KeyError()")
+        self.assertEqual(500, expected_response.status_code)
+        self.assertEqual(response.body, expected_response.body)
+
 
 if __name__ == "__main__":
     unittest.main()
```

