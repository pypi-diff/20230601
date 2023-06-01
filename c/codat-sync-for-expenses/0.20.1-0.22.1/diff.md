# Comparing `tmp/codat-sync-for-expenses-0.20.1.tar.gz` & `tmp/codat-sync-for-expenses-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.20.1.tar", last modified: Mon May 22 17:58:20 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.22.1.tar", last modified: Thu Jun  1 16:45:57 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.20.1.tar` & `codat-sync-for-expenses-0.22.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2560 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 17:58:20.000000 codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4736 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2582 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4739 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2511 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.859077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1214 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1786 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5685 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/integrationtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7325 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4342 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:58:20.863077 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-05-22 17:58:08.000000 codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2573 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.759792 codat-sync-for-expenses-0.22.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5291 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2782 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5695 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8409 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.20.1/PKG-INFO` & `codat-sync-for-expenses-0.22.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.20.1
+Version: 0.22.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # Sync for Expenses
 
 Embedded accounting integrations for corporate card providers.
 
 <!-- Start SDK Installation -->
 ## SDK Installation
@@ -25,15 +26,15 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsyncexpenses
 from codatsyncexpenses.models import operations
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
-        auth_header="YOUR_API_KEY_HERE",
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
     ),
 )
 
 req = operations.GetCompanyConfigurationRequest(
     company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
```

### Comparing `codat-sync-for-expenses-0.20.1/README.md` & `codat-sync-for-expenses-0.22.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsyncexpenses
 from codatsyncexpenses.models import operations
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
-        auth_header="YOUR_API_KEY_HERE",
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
     ),
 )
 
 req = operations.GetCompanyConfigurationRequest(
     company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
```

### Comparing `codat-sync-for-expenses-0.20.1/setup.py` & `codat-sync-for-expenses-0.22.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,37 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.20.1",
+    version="0.22.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi==2022.12.7",
-        "charset-normalizer==2.1.1",
-        "dataclasses-json-speakeasy==0.5.8",
-        "idna==3.3",
-        "marshmallow==3.17.1",
-        "marshmallow-enum==1.5.1",
-        "mypy-extensions==0.4.3",
-        "packaging==21.3",
-        "pyparsing==3.0.9",
-        "python-dateutil==2.8.2",
-        "requests==2.28.1",
-        "six==1.16.0",
-        "typing-inspect==0.8.0",
-        "typing_extensions==4.3.0",
-        "urllib3==1.26.12",
-        "pylint==2.16.2",
+        "certifi>=2022.12.7",
+        "charset-normalizer>=2.1.1",
+        "dataclasses-json-speakeasy>=0.5.8",
+        "idna>=3.3",
+        "jsonpath-python>=1.0.6 ",
+        "marshmallow>=3.17.1",
+        "marshmallow-enum>=1.5.1",
+        "mypy-extensions>=0.4.3",
+        "packaging>=21.3",
+        "pyparsing>=3.0.9",
+        "python-dateutil>=2.8.2",
+        "requests>=2.28.1",
+        "six>=1.16.0",
+        "typing-inspect>=0.8.0",
+        "typing_extensions>=4.3.0",
+        "urllib3>=1.26.12",
     ],
+    extras_require={
+        "dev":["pylint==2.16.2"]
+    },
     package_dir={'': 'src'},
     python_requires='>=3.9'
 )
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.20.1
+Version: 0.22.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # Sync for Expenses
 
 Embedded accounting integrations for corporate card providers.
 
 <!-- Start SDK Installation -->
 ## SDK Installation
@@ -25,15 +26,15 @@
 <!-- Start SDK Example Usage -->
 ```python
 import codatsyncexpenses
 from codatsyncexpenses.models import operations
 
 s = codatsyncexpenses.CodatSyncExpenses(
     security=shared.Security(
-        auth_header="YOUR_API_KEY_HERE",
+        auth_header="Basic BASE_64_ENCODED(API_KEY)",
     ),
 )
 
 req = operations.GetCompanyConfigurationRequest(
     company_id='8a210b68-6988-11ed-a1eb-0242ac120002',
 )
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 src/codatsyncexpenses/models/shared/expensetransaction.py
 src/codatsyncexpenses/models/shared/expensetransactionline.py
 src/codatsyncexpenses/models/shared/hallink.py
 src/codatsyncexpenses/models/shared/integrationtype.py
 src/codatsyncexpenses/models/shared/mappingoptions.py
 src/codatsyncexpenses/models/shared/postsync.py
 src/codatsyncexpenses/models/shared/recordref.py
+src/codatsyncexpenses/models/shared/schema.py
 src/codatsyncexpenses/models/shared/security.py
 src/codatsyncexpenses/models/shared/supplier.py
 src/codatsyncexpenses/models/shared/syncinitiated.py
 src/codatsyncexpenses/models/shared/taxratemappinginfo.py
 src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
 src/codatsyncexpenses/models/shared/transactionmetadata.py
 src/codatsyncexpenses/models/shared/transactionmetadatalist.py
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -54,14 +54,18 @@
 
         res = operations.GetCompanyConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyConfiguration])
                 res.company_configuration = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def save_company_configuration(self, request: operations.SaveCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SaveCompanyConfigurationResponse:
         r"""Set company configuration
         Sets a companies expense sync configuration
@@ -96,15 +100,15 @@
 
         res = operations.SaveCompanyConfigurationResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanyConfiguration])
                 res.company_configuration = out
-        elif http_res.status_code == 400:
+        elif http_res.status_code in [400, 401, 404, 429]:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CodatErrorMessage])
-                res.codat_error_message = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/connections.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""Create Partner Expense connection
         Creates a Partner Expense data connection
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -54,11 +54,15 @@
 
         res = operations.CreatePartnerExpenseConnectionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.DataConnection])
                 res.data_connection = out
+        elif http_res.status_code in [400, 401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/expenses.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -57,14 +57,18 @@
 
         res = operations.CreateExpenseDatasetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateExpenseResponse])
                 res.create_expense_response = out
+        elif http_res.status_code in [400, 401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def upload_attachment(self, request: operations.UploadAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadAttachmentResponse:
         r"""Upload attachment
         Creates an attachment in the accounting software against the given transactionId
@@ -72,15 +76,15 @@
         base_url = self._server_url
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -99,11 +103,15 @@
 
         res = operations.UploadAttachmentResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Attachment])
                 res.attachment = out
+        elif http_res.status_code in [400, 401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/mapping_options.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""Mapping options
         Gets the expense mapping options for a companies accounting software
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -54,11 +54,15 @@
 
         res = operations.GetMappingOptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MappingOptions])
                 res.mapping_options = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import createexpenserequest as shared_createexpenserequest
 from ..shared import createexpenseresponse as shared_createexpenseresponse
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateExpenseDatasetRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
@@ -19,8 +20,10 @@
 class CreateExpenseDatasetResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     create_expense_response: Optional[shared_createexpenseresponse.CreateExpenseResponse] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""The request made is not valid."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import dataconnection as shared_dataconnection
+from ..shared import mappingoptions as shared_mappingoptions
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreatePartnerExpenseConnectionRequest:
+class GetMappingOptionsRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
 @dataclasses.dataclass
-class CreatePartnerExpenseConnectionResponse:
+class GetMappingOptionsResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    data_connection: Optional[shared_dataconnection.DataConnection] = dataclasses.field(default=None)
+    mapping_options: Optional[shared_mappingoptions.MappingOptions] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import companyconfiguration as shared_companyconfiguration
+from ..shared import companysyncstatus as shared_companysyncstatus
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetCompanyConfigurationRequest:
+class ListSyncsRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
 @dataclasses.dataclass
-class GetCompanyConfigurationResponse:
+class ListSyncsResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
+    company_sync_statuses: Optional[list[shared_companysyncstatus.CompanySyncStatus]] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLastSuccessfulSyncRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
@@ -17,8 +18,10 @@
 class GetLastSuccessfulSyncResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetLatestSyncRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
@@ -17,8 +18,10 @@
 class GetLatestSyncResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import companysyncstatus as shared_companysyncstatus
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncByIDRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
@@ -19,8 +20,10 @@
 class GetSyncByIDResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     company_sync_status: Optional[shared_companysyncstatus.CompanySyncStatus] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import schema as shared_schema
 from ..shared import transactionmetadata as shared_transactionmetadata
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetSyncTransactionRequest:
     
@@ -19,10 +20,12 @@
 
 @dataclasses.dataclass
 class GetSyncTransactionResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
     transaction_metadata: Optional[list[shared_transactionmetadata.TransactionMetadata]] = dataclasses.field(default=None)
     r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
+from ..shared import schema as shared_schema
 from ..shared import transactionmetadatalist as shared_transactionmetadatalist
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSyncTransactionsRequest:
     
@@ -21,10 +22,12 @@
 
 @dataclasses.dataclass
 class ListSyncTransactionsResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
     transaction_metadata_list: Optional[shared_transactionmetadatalist.TransactionMetadataList] = dataclasses.field(default=None)
     r"""Success"""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import companysyncstatus as shared_companysyncstatus
+from ..shared import companyconfiguration as shared_companyconfiguration
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListSyncsRequest:
+class GetCompanyConfigurationRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
     
 
 @dataclasses.dataclass
-class ListSyncsResponse:
+class GetCompanyConfigurationResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    company_sync_statuses: Optional[list[shared_companysyncstatus.CompanySyncStatus]] = dataclasses.field(default=None)
+    company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""Your API request was not properly authorized."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import codaterrormessage as shared_codaterrormessage
 from ..shared import companyconfiguration as shared_companyconfiguration
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationRequest:
     
     company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
@@ -16,13 +16,13 @@
     
 
 @dataclasses.dataclass
 class SaveCompanyConfigurationResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-    codat_error_message: Optional[shared_codaterrormessage.CodatErrorMessage] = dataclasses.field(default=None)
-    r"""Bad Request"""
     company_configuration: Optional[shared_companyconfiguration.CompanyConfiguration] = dataclasses.field(default=None)
     r"""Success"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""The request made is not valid."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ..shared import attachment as shared_attachment
+from ..shared import schema as shared_schema
 from typing import Optional
 
 
 @dataclasses.dataclass
 class UploadAttachmentRequestBody:
     
     content: bytes = dataclasses.field(metadata={'multipart_form': { 'content': True }})
@@ -29,8 +30,10 @@
 class UploadAttachmentResponse:
     
     content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
     attachment: Optional[shared_attachment.Attachment] = dataclasses.field(default=None)
     r"""OK"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    schema: Optional[shared_schema.Schema] = dataclasses.field(default=None)
+    r"""The request made is not valid."""
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 from .expensetransaction import *
 from .expensetransactionline import *
 from .hallink import *
 from .integrationtype import *
 from .mappingoptions import *
 from .postsync import *
 from .recordref import *
+from .schema import *
 from .security import *
 from .supplier import *
 from .syncinitiated import *
 from .taxratemappinginfo import *
 from .trackingcategorymappinginfo import *
 from .transactionmetadata import *
 from .transactionmetadatalist import *
 from .transactionstatus import *
 
-__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountMappingInfoValidTransactionTypes","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceType","DataConnectionStatus","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","HalLink","IntegrationType","MappingOptions","PostSync","RecordRef","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatus"]
+__all__ = ["AccountMappingInfo","AccountMappingInfoAccountType","AccountMappingInfoValidTransactionTypes","Attachment","BankAccount","CodatErrorMessage","CodatErrorMessageValidation","CodatErrorMessageValidationErrors","CodatErrorMessageValidationInternals","CodatErrorMessageValidationWarnings","CompanyConfiguration","CompanySyncStatus","CreateExpenseRequest","CreateExpenseResponse","Customer","DataConnection","DataConnectionError","DataConnectionSourceType","DataConnectionStatus","ExpenseTransaction","ExpenseTransactionLine","ExpenseTransactionType","HalLink","IntegrationType","MappingOptions","PostSync","RecordRef","Schema","Security","Supplier","SyncInitiated","TaxRateMappingInfo","TaxRateMappingInfoValidTransactionTypes","TrackingCategoryMappingInfo","TransactionMetadata","TransactionMetadataList","TransactionMetadataListLinks","TransactionStatus"]
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     internals: Optional[list[CodatErrorMessageValidationInternals]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('internals'), 'exclude': lambda f: f is None }})
     warnings: Optional[list[CodatErrorMessageValidationWarnings]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warnings'), 'exclude': lambda f: f is None }})
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CodatErrorMessage:
-    r"""Bad Request"""
+    r"""If model is incorrect"""
     
     can_be_retried: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('canBeRetried'), 'exclude': lambda f: f is None }})
     correlation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('correlationId'), 'exclude': lambda f: f is None }})
     detailed_error_code: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailedErrorCode'), 'exclude': lambda f: f is None }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     inner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inner'), 'exclude': lambda f: f is None }})
     service: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sdk.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     transaction_status: TransactionStatus
     r"""Retrieve the status of transactions within a sync."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.20.1"
-    _gen_version: str = "2.31.0"
+    _sdk_version: str = "0.22.1"
+    _gen_version: str = "2.34.7"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""Last successful sync
         Gets the status of the last successfull sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -54,27 +54,31 @@
 
         res = operations.GetLastSuccessfulSyncResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def get_latest_sync(self, request: operations.GetLatestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLatestSyncResponse:
         r"""Latest sync status
         Gets the latest sync status
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -93,27 +97,31 @@
 
         res = operations.GetLatestSyncResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def get_sync_by_id(self, request: operations.GetSyncByIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncByIDResponse:
         r"""Get Sync status
         Get the sync status for a specified sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -132,27 +140,31 @@
 
         res = operations.GetSyncByIDResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CompanySyncStatus])
                 res.company_sync_status = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def list_syncs(self, request: operations.ListSyncsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncsResponse:
         r"""List sync statuses
         Gets a list of sync statuses
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -171,11 +183,15 @@
 
         res = operations.ListSyncsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[list[shared.CompanySyncStatus]])
                 res.company_sync_statuses = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/transaction_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         r"""Get Sync Transaction
         Gets the status of a transaction for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         headers = {}
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -54,28 +54,32 @@
 
         res = operations.GetSyncTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[list[shared.TransactionMetadata]])
                 res.transaction_metadata = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
 
     
     def list_sync_transactions(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
         r"""Get Sync transactions
         Get's the transactions and status for a sync
         """
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
-        headers['Accept'] = 'application/json'
+        headers['Accept'] = 'application/json;q=1, application/json;q=0'
         headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
         
         client = self._security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
@@ -94,11 +98,15 @@
 
         res = operations.ListSyncTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionMetadataList])
                 res.transaction_metadata_list = out
+        elif http_res.status_code in [401, 404, 429]:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.20.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

