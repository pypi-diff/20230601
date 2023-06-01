# Comparing `tmp/tc-messageBroker-1.1.2.tar.gz` & `tmp/tc-messageBroker-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.1.2.tar", last modified: Tue May 30 15:45:40 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.1.3.tar", last modified: Thu Jun  1 07:46:04 2023, max compression
```

## Comparing `tc-messageBroker-1.1.2.tar` & `tc-messageBroker-1.1.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.614549 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 15:45:40.000000 tc-messageBroker-1.1.2/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.618548 tc-messageBroker-1.1.2/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:40.622549 tc-messageBroker-1.1.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-30 15:45:19.000000 tc-messageBroker-1.1.2/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.2/PKG-INFO` & `tc-messageBroker-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.2/README.md` & `tc-messageBroker-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/setup.py` & `tc-messageBroker-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.1.2",
+    version="1.1.3",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.1.3/tc_messageBroker/message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,18 +223,18 @@
             the dictionary representing the current saga document
 
         """
         data = {}
 
         data["choreography"] = {}
         data["choreography"]["name"] = self.choreography.name
-        data["choreography"]["transactions"] = {}
-        for idx, tx in enumerate(self.choreography.transactions):
+        data["choreography"]["transactions"] = []
+        for tx in self.choreography.transactions:
             transaction = convert_tx_dict(tx)
-            data["choreography"]["transactions"][str(idx)] = transaction
+            data["choreography"]["transactions"].append(transaction)
 
         data["status"] = self.status
         data["data"] = self.data
         data["sagaId"] = self.uuid
         data["createdAt"] = self.created_at
         data["updatedAt"] = datetime.now()
 
@@ -250,22 +250,22 @@
             db_name=mongo_creds["db_name"],
             collection_name=mongo_creds["collection_name"],
         )
         mongodb.connect()
         return mongodb
 
 
-def get_saga(guildId: str, connection_url: str, db_name: str, collection: str):
+def get_saga(sagaId: str, connection_url: str, db_name: str, collection: str):
     """
     get saga object for a special guild
 
     Parameters:
     ------------
-    guildId : str
-        the guildId which the saga belongs to
+    sagaId : str
+        the sagaId which the saga belongs to
     connection_url : str
         the connection to db which the saga architecture is saved
     db_name : str
         the database name to use
     collection : str
         the collection which the saga is saved
 
@@ -275,29 +275,28 @@
         the saga object to use
     """
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection
     )
     mongodb.connect()
 
-    data = mongodb.read(query={"data.guildId": guildId}, count=1)
-
-    transactions = get_transactions(data["choreography"]["transactions"])
-
-    choreography = IChoreography(
-        name=data["choreography"]["name"],
-        transactions=transactions,
-    )
+    data = mongodb.read(query={"sagaId": sagaId}, count=1)
 
     saga_obj = None
-    if data is not None:
+    try:
+        transactions = get_transactions(data["choreography"]["transactions"])
+
+        choreography = IChoreography(
+            name=data["choreography"]["name"],
+            transactions=transactions,
+        )
         saga_obj = Saga(
             choreography=choreography,
             status=data["status"],
             created_at=data["createdAt"],
             sagaId=data["sagaId"],
             data=data["data"],
         )
-    else:
-        logging.error("Error! no saga available for this!")
+    except Exception as exp:
+        logging.error(f"Error occured! Exception: {exp}")
 
     return saga_obj
```

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,16 @@
         "choreography": {
             "type": "object",
             "properties": {
                 "name": {
                     "type": "string",
                 },
                 "transactions": {
-                    "type": "object",
-                    "patternProperties": {
-                        "^[0-9]+$": {
+                    "type": "array",
+                    "items": {
                             "type": "object",
                             "properties": {
                                 "queue": {"type": "string"},
                                 "event": {"type": "string"},
                                 "order": {"type": ["integer", "string"]},
                                 "status": {
                                     "type": "string",
@@ -33,15 +32,14 @@
                                 "start": {},
                                 "end": {},
                                 "runtime": {"type": "number"},
                                 "error": {"type": "string"},
                             },
                             "required": ["queue", "event", "order", "status"],
                             "additionalProperties": False,
-                        }
                     },
                     "additionalProperties": False,
                 },
             },
             "required": ["name", "transactions"],
             "additionalProperties": False,
         },
```

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Doing the object to dict and vice operations here
 from tc_messageBroker.rabbit_mq.saga.transactions import ITransaction
 
 
 def get_transactions(transactions: dict[dict[str, any]]) -> list[ITransaction]:
     transactions_obj = []
 
-    for tx in transactions.values():
+    for tx in transactions:
         transaction = ITransaction(**tx)
         transactions_obj.append(transaction)
 
     return transactions_obj
 
 
 def convert_tx_dict(transaction: ITransaction):
```

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.1.3/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.2/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.1.3/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.1.3/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/integration/test_mongodb.py` & `tc-messageBroker-1.1.3/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/integration/test_saga.py` & `tc-messageBroker-1.1.3/tests/integration/test_saga.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     reason="Unable to test on GitHub Actions (no available MongoDB instance)"
 )
 def test_inputs():
     connection_url = "mongodb://127.0.0.1:27017/"
 
     ## we should have this data before running this test in db
     saga = get_saga(
-        guildId="993163081939165234",
+        sagaId="something",
         connection_url=connection_url,
         db_name="Saga",
         collection="saga",
     )
 
     assert saga.choreography is not None
     assert saga.status in [
```

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.1.3/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_message_broker.py` & `tc-messageBroker-1.1.3/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.1.3/tests/unit/test_predefined_transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_saga_base.py` & `tc-messageBroker-1.1.3/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_saga_base_utils.py` & `tc-messageBroker-1.1.3/tests/unit/test_saga_base_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,44 +85,44 @@
 
 def test_get_transactions_length():
     event = "EVENT"
     queue = "QUEUE"
     order = 1
     status = "STATUS"
 
-    transactions = {}
+    transactions = []
     loop_iter = 2
     for i in range(loop_iter):
         tx = {}
         tx["event"] = event + str(i)
         tx["queue"] = queue + str(i)
         tx["order"] = order + i
         tx["status"] = status + str(i)
 
-        transactions[str(i)] = tx
+        transactions.append(tx)
 
     transactions_obj = get_transactions(transactions)
 
     assert len(transactions_obj) == loop_iter
 
 
 def test_get_transactions_obj():
     event = "EVENT"
     queue = "QUEUE"
     order = 1
     status = "STATUS"
 
-    transactions = {}
+    transactions = []
     loop_iter = 2
     for i in range(loop_iter):
         tx = {}
         tx["event"] = event + str(i)
         tx["queue"] = queue + str(i)
         tx["order"] = order + i
         tx["status"] = status + str(i)
 
-        transactions[str(i)] = tx
+        transactions.append(tx)
 
     transactions_obj = get_transactions(transactions)
 
     for i in range(loop_iter):
         assert isinstance(transactions_obj[i], ITransaction) is True
```

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_saga_next.py` & `tc-messageBroker-1.1.3/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_saga_start.py` & `tc-messageBroker-1.1.3/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.2/tests/unit/test_transactions.py` & `tc-messageBroker-1.1.3/tests/unit/test_transactions.py`

 * *Files identical despite different names*

