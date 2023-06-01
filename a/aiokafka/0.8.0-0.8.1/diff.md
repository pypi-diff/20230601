# Comparing `tmp/aiokafka-0.8.0.tar.gz` & `tmp/aiokafka-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiokafka-0.8.0.tar", last modified: Mon Nov 21 14:04:38 2022, max compression
+gzip compressed data, was "aiokafka-0.8.1.tar", last modified: Thu Jun  1 13:38:26 2023, max compression
```

## Comparing `aiokafka-0.8.0.tar` & `aiokafka-0.8.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    14053 2022-11-21 14:04:15.000000 aiokafka-0.8.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11348 2022-11-21 14:04:15.000000 aiokafka-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-11-21 14:04:15.000000 aiokafka-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18608 2022-11-21 14:04:38.000000 aiokafka-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3435 2022-11-21 14:04:15.000000 aiokafka-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6094 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)    24651 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    27766 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    28600 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/conn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/consumer/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55682 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/consumer/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)    49461 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/consumer/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    59886 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/consumer/group_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (121)    18801 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/consumer/subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (121)    12834 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3408 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/producer/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17674 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/producer/message_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (121)    27851 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/producer/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)    33194 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/producer/sender.py
--rw-r--r--   0 runner    (1001) docker     (121)     8243 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/producer/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/protocol/coordination.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/protocol/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/record/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5610 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crc32c.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka/record/_crecords/
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/consts.pxi
--rw-r--r--   0 runner    (1001) docker     (121)    12034 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/crc32c.c
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/crc32c.h
--rw-r--r--   0 runner    (1001) docker     (121)   280843 2022-11-21 14:04:23.000000 aiokafka-0.8.0/aiokafka/record/_crecords/cutil.c
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/cutil.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/cutil.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   814715 2022-11-21 14:04:24.000000 aiokafka-0.8.0/aiokafka/record/_crecords/default_records.c
--rw-r--r--   0 runner    (1001) docker     (121)     1423 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/default_records.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    28732 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/default_records.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/hton.pxd
--rw-r--r--   0 runner    (1001) docker     (121)   702879 2022-11-21 14:04:24.000000 aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.c
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    19046 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.pyx
--rw-r--r--   0 runner    (1001) docker     (121)   257791 2022-11-21 14:04:25.000000 aiokafka-0.8.0/aiokafka/record/_crecords/memory_records.c
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/_crecords/memory_records.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/control_record.py
--rw-r--r--   0 runner    (1001) docker     (121)    22400 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/default_records.py
--rw-r--r--   0 runner    (1001) docker     (121)    17412 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/legacy_records.py
--rw-r--r--   0 runner    (1001) docker     (121)     3378 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/memory_records.py
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/record/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/structs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-11-21 14:04:15.000000 aiokafka-0.8.0/aiokafka/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18608 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-21 14:04:38.000000 aiokafka-0.8.0/aiokafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-11-21 14:04:38.000000 aiokafka-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5390 2022-11-21 14:04:15.000000 aiokafka-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.206817 aiokafka-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    14478 2023-06-01 13:38:14.000000 aiokafka-0.8.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-01 13:38:14.000000 aiokafka-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 13:38:14.000000 aiokafka-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-01 13:38:26.206817 aiokafka-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-01 13:38:14.000000 aiokafka-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.194816 aiokafka-0.8.1/aiokafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25357 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27766 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/conn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.198816 aiokafka-0.8.1/aiokafka/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55870 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/consumer/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/consumer/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59886 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/consumer/group_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18801 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/consumer/subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.198816 aiokafka-0.8.1/aiokafka/producer/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/producer/message_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/producer/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33194 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/producer/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/producer/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.198816 aiokafka-0.8.1/aiokafka/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/protocol/coordination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/protocol/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.198816 aiokafka-0.8.1/aiokafka/record/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crc32c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.206817 aiokafka-0.8.1/aiokafka/record/_crecords/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/consts.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/crc32c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/crc32c.h
+-rw-r--r--   0 runner    (1001) docker     (123)   280843 2023-06-01 13:38:24.000000 aiokafka-0.8.1/aiokafka/record/_crecords/cutil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/cutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/cutil.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   814715 2023-06-01 13:38:25.000000 aiokafka-0.8.1/aiokafka/record/_crecords/default_records.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/default_records.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    28732 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/default_records.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/hton.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   702879 2023-06-01 13:38:25.000000 aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.c
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19046 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   257791 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka/record/_crecords/memory_records.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/_crecords/memory_records.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/control_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22400 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/default_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17412 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/legacy_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/memory_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/record/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-01 13:38:14.000000 aiokafka-0.8.1/aiokafka/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:38:26.198816 aiokafka-0.8.1/aiokafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 13:38:26.000000 aiokafka-0.8.1/aiokafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 13:38:26.206817 aiokafka-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-01 13:38:14.000000 aiokafka-0.8.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiokafka-0.8.0/CHANGES.rst` & `aiokafka-0.8.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,34 @@
 =========
 Changelog
 =========
 
 
+0.8.1 (2023-05-31)
+==================
+
+New features:
+
+* Drop support for Python 3.7 due to end of life (pr #893)
+
+
+Bugfixes:
+
+* Add SASL authentication support to `AIOKafkaAdminClient` (issue #889,
+  pr #890 by @selevit)
+
+
+Improved Documentation:
+
+* Update `security_protocol` argument docstring (issue #883, pr #884 by
+  @gabrielmbmb)
+* Remove incorrect `await` for `AIOKafkaConsumer.highwater()` (pr #858 by
+  @yi-jiayu)
+
+
 0.8.0 (2022-11-21)
 ==================
 
 New features:
 
 * Add codec for ZStandard compression (KIP-110) (pr #801)
 * Add basic admin client functionality (pr #811 started by @gabriel-tincu)
```

### Comparing `aiokafka-0.8.0/LICENSE` & `aiokafka-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/PKG-INFO` & `aiokafka-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: aiokafka
-Version: 0.8.0
+Version: 0.8.1
 Summary: Kafka integration with asyncio.
 Home-page: http://aiokafka.readthedocs.org
 Download-URL: https://pypi.python.org/pypi/aiokafka
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache 2
 Project-URL: Source, https://github.com/aio-libs/aiokafka
 Platform: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Framework :: AsyncIO
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: snappy
 Provides-Extra: lz4
 Provides-Extra: zstd
 Provides-Extra: gssapi
 Provides-Extra: all
 License-File: LICENSE
 
@@ -109,15 +108,15 @@
 Docker is required to run tests. See https://docs.docker.com/engine/installation for installation notes. Also note, that `lz4` compression libraries for python will require `python-dev` package,
 or python source header files for compilation on Linux.
 NOTE: You will also need a valid java installation. It's required for the ``keytool`` utility, used to
 generate ssh keys for some tests.
 
 Setting up tests requirements (assuming you're within virtualenv on ubuntu 14.04+)::
 
-    sudo apt-get install -y libsnappy-dev libzstd-dev
+    sudo apt-get install -y libsnappy-dev libzstd-dev libkrb5-dev krb5-user
     make setup
 
 Running tests with coverage::
 
     make cov
 
 To run tests with a specific version of Kafka (default one is 1.0.2) use KAFKA_VERSION variable::
@@ -132,14 +131,36 @@
  * ``make test FLAGS="--no-pull"`` - do not try to pull new docker image before test run.
 
 =========
 Changelog
 =========
 
 
+0.8.1 (2023-05-31)
+==================
+
+New features:
+
+* Drop support for Python 3.7 due to end of life (pr #893)
+
+
+Bugfixes:
+
+* Add SASL authentication support to `AIOKafkaAdminClient` (issue #889,
+  pr #890 by @selevit)
+
+
+Improved Documentation:
+
+* Update `security_protocol` argument docstring (issue #883, pr #884 by
+  @gabrielmbmb)
+* Remove incorrect `await` for `AIOKafkaConsumer.highwater()` (pr #858 by
+  @yi-jiayu)
+
+
 0.8.0 (2022-11-21)
 ==================
 
 New features:
 
 * Add codec for ZStandard compression (KIP-110) (pr #801)
 * Add basic admin client functionality (pr #811 started by @gabriel-tincu)
```

### Comparing `aiokafka-0.8.0/README.rst` & `aiokafka-0.8.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 Docker is required to run tests. See https://docs.docker.com/engine/installation for installation notes. Also note, that `lz4` compression libraries for python will require `python-dev` package,
 or python source header files for compilation on Linux.
 NOTE: You will also need a valid java installation. It's required for the ``keytool`` utility, used to
 generate ssh keys for some tests.
 
 Setting up tests requirements (assuming you're within virtualenv on ubuntu 14.04+)::
 
-    sudo apt-get install -y libsnappy-dev libzstd-dev
+    sudo apt-get install -y libsnappy-dev libzstd-dev libkrb5-dev krb5-user
     make setup
 
 Running tests with coverage::
 
     make cov
 
 To run tests with a specific version of Kafka (default one is 1.0.2) use KAFKA_VERSION variable::
```

### Comparing `aiokafka-0.8.0/aiokafka/__init__.py` & `aiokafka-0.8.1/aiokafka/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.0'  # noqa
+__version__ = '0.8.1'  # noqa
 
 from .abc import ConsumerRebalanceListener
 from .client import AIOKafkaClient
 from .consumer import AIOKafkaConsumer
 from .errors import ConsumerStoppedError, IllegalOperation
 from .producer import AIOKafkaProducer
 from .structs import (
```

### Comparing `aiokafka-0.8.0/aiokafka/abc.py` & `aiokafka-0.8.1/aiokafka/abc.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/admin.py` & `aiokafka-0.8.1/aiokafka/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,28 +77,40 @@
                  client_id: str = 'aiokafka-' + __version__,
                  request_timeout_ms: int = 40000,
                  connections_max_idle_ms: int = 540000,
                  retry_backoff_ms: int = 100,
                  metadata_max_age_ms: int = 300000,
                  security_protocol: str = "PLAINTEXT",
                  ssl_context: Optional[SSLContext] = None,
-                 api_version: str = "auto"):
+                 api_version: str = "auto",
+                 sasl_mechanism: str = 'PLAIN',
+                 sasl_plain_username: Optional[str] = None,
+                 sasl_plain_password: Optional[str] = None,
+                 sasl_kerberos_service_name: str = 'kafka',
+                 sasl_kerberos_domain_name: Optional[str] = None,
+                 sasl_oauth_token_provider: Optional[str] = None):
         self._closed = False
         self._started = False
         self._version_info = {}
         self._request_timeout_ms = request_timeout_ms
         self._client = AIOKafkaClient(
             loop=loop, bootstrap_servers=bootstrap_servers,
             client_id=client_id, metadata_max_age_ms=metadata_max_age_ms,
             request_timeout_ms=request_timeout_ms,
             retry_backoff_ms=retry_backoff_ms,
             api_version=api_version,
             ssl_context=ssl_context,
             security_protocol=security_protocol,
-            connections_max_idle_ms=connections_max_idle_ms)
+            connections_max_idle_ms=connections_max_idle_ms,
+            sasl_mechanism=sasl_mechanism,
+            sasl_plain_username=sasl_plain_username,
+            sasl_plain_password=sasl_plain_password,
+            sasl_kerberos_service_name=sasl_kerberos_service_name,
+            sasl_kerberos_domain_name=sasl_kerberos_domain_name,
+            sasl_oauth_token_provider=sasl_oauth_token_provider)
 
     async def close(self):
         """Close the KafkaAdminClient connection to the Kafka broker."""
         if not hasattr(self, '_closed') or self._closed:
             log.info("KafkaAdminClient already closed.")
             return
```

### Comparing `aiokafka-0.8.0/aiokafka/client.py` & `aiokafka-0.8.1/aiokafka/client.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/cluster.py` & `aiokafka-0.8.1/aiokafka/cluster.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/conn.py` & `aiokafka-0.8.1/aiokafka/conn.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/consumer/consumer.py` & `aiokafka-0.8.1/aiokafka/consumer/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 import logging
 import re
 import sys
 import traceback
 import warnings
+from typing import Dict, List
 
 from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 
 from aiokafka.abc import ConsumerRebalanceListener
 from aiokafka.client import AIOKafkaClient
 from aiokafka.errors import (
     TopicAuthorizationFailedError, OffsetOutOfRangeError,
     ConsumerStoppedError, IllegalOperation, UnsupportedVersionError,
     IllegalStateError, NoOffsetForPartitionError, RecordTooLargeError
 )
-from aiokafka.structs import TopicPartition
+from aiokafka.structs import TopicPartition, ConsumerRecord
 from aiokafka.util import (
     commit_structure_validate, get_running_loop
 )
 from aiokafka import __version__
 
 from .fetcher import Fetcher, OffsetResetStrategy
 from .group_coordinator import GroupCoordinator, NoGroupCoordinator
@@ -163,15 +164,16 @@
             routine. Mostly defines how fast the system will see rebalance and
             request new data for new partitions. Default: 200
         api_version (str): specify which kafka API version to use.
             :class:`AIOKafkaConsumer` supports Kafka API versions >=0.9 only.
             If set to ``auto``, will attempt to infer the broker version by
             probing various APIs. Default: ``auto``
         security_protocol (str): Protocol used to communicate with brokers.
-            Valid values are: ``PLAINTEXT``, ``SSL``. Default: ``PLAINTEXT``.
+            Valid values are: ``PLAINTEXT``, ``SSL``, ``SASL_PLAINTEXT``,
+            ``SASL_SSL``. Default: ``PLAINTEXT``.
         ssl_context (ssl.SSLContext): pre-configured :class:`~ssl.SSLContext`
             for wrapping socket connections. Directly passed into asyncio's
             :meth:`~asyncio.loop.create_connection`. For more information see
             :ref:`ssl_auth`. Default: None.
         exclude_internal_topics (bool): Whether records from internal topics
             (such as offsets) should be exposed to the consumer. If set to True
             the only way to receive records from an internal topic is
@@ -259,15 +261,15 @@
                  sasl_kerberos_service_name='kafka',
                  sasl_kerberos_domain_name=None,
                  sasl_oauth_token_provider=None):
         if loop is None:
             loop = get_running_loop()
         else:
             warnings.warn("The loop argument is deprecated since 0.7.1, "
-                          "and scheduled for removal in 0.8.0",
+                          "and scheduled for removal in 0.9.0",
                           DeprecationWarning, stacklevel=2)
 
         if max_poll_records is not None and (
                 not isinstance(max_poll_records, int) or max_poll_records < 1):
             raise ValueError("`max_poll_records` should be positive Integer")
 
         if rebalance_timeout_ms is None:
@@ -1100,15 +1102,15 @@
         self._subscription.unsubscribe()
         if self._group_id is not None:
             self._coordinator.maybe_leave_group()
         self._client.set_topics([])
         log.info(
             "Unsubscribed all topics or patterns and assigned partitions")
 
-    async def getone(self, *partitions):
+    async def getone(self, *partitions) -> ConsumerRecord:
         """
         Get one message from Kafka.
         If no new messages prefetched, this method will wait for it.
 
         Arguments:
             partitions (list(TopicPartition)): Optional list of partitions to
                 return from. If no partitions specified then returned message
@@ -1144,15 +1146,17 @@
         # Raise coordination errors if any
         self._coordinator.check_errors()
 
         with self._subscription.fetch_context():
             msg = await self._fetcher.next_record(partitions)
         return msg
 
-    async def getmany(self, *partitions, timeout_ms=0, max_records=None):
+    async def getmany(
+        self, *partitions, timeout_ms=0, max_records=None
+    ) -> Dict[TopicPartition, List[ConsumerRecord]]:
         """Get messages from assigned topics / partitions.
 
         Prefetched messages are returned in batches by topic-partition.
         If messages is not available in the prefetched buffer this method waits
         `timeout_ms` milliseconds.
 
         Arguments:
@@ -1243,15 +1247,15 @@
             self._subscription.resume(partition)
 
     def __aiter__(self):
         if self._closed:
             raise ConsumerStoppedError()
         return self
 
-    async def __anext__(self):
+    async def __anext__(self) -> ConsumerRecord:
         """Asyncio iterator interface for consumer
 
         Note:
             TopicAuthorizationFailedError and OffsetOutOfRangeError
             exceptions can be raised in iterator.
             All other KafkaError exceptions will be logged and not raised
         """
```

### Comparing `aiokafka-0.8.0/aiokafka/consumer/fetcher.py` & `aiokafka-0.8.1/aiokafka/consumer/fetcher.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/consumer/group_coordinator.py` & `aiokafka-0.8.1/aiokafka/consumer/group_coordinator.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/consumer/subscription_state.py` & `aiokafka-0.8.1/aiokafka/consumer/subscription_state.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/errors.py` & `aiokafka-0.8.1/aiokafka/errors.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/helpers.py` & `aiokafka-0.8.1/aiokafka/helpers.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/producer/message_accumulator.py` & `aiokafka-0.8.1/aiokafka/producer/message_accumulator.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/producer/producer.py` & `aiokafka-0.8.1/aiokafka/producer/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,16 @@
             Default: 40000.
         retry_backoff_ms (int): Milliseconds to backoff when retrying on
             errors. Default: 100.
         api_version (str): specify which kafka API version to use.
             If set to ``auto``, will attempt to infer the broker version by
             probing various APIs. Default: ``auto``
         security_protocol (str): Protocol used to communicate with brokers.
-            Valid values are: ``PLAINTEXT``, ``SSL``. Default: ``PLAINTEXT``.
-            Default: ``PLAINTEXT``.
+            Valid values are: ``PLAINTEXT``, ``SSL``, ``SASL_PLAINTEXT``,
+            ``SASL_SSL``. Default: ``PLAINTEXT``.
         ssl_context (ssl.SSLContext): pre-configured :class:`~ssl.SSLContext`
             for wrapping socket connections. Directly passed into asyncio's
             :meth:`~asyncio.loop.create_connection`. For more
             information see :ref:`ssl_auth`.
             Default: :data:`None`
         connections_max_idle_ms (int): Close idle connections after the number
             of milliseconds specified by this config. Specifying :data:`None` will
@@ -202,15 +202,15 @@
                  sasl_kerberos_service_name='kafka',
                  sasl_kerberos_domain_name=None,
                  sasl_oauth_token_provider=None):
         if loop is None:
             loop = get_running_loop()
         else:
             warnings.warn("The loop argument is deprecated since 0.7.1, "
-                          "and scheduled for removal in 0.8.0",
+                          "and scheduled for removal in 0.9.0",
                           DeprecationWarning, stacklevel=2)
         if loop.get_debug():
             self._source_traceback = traceback.extract_stack(sys._getframe(1))
         self._loop = loop
 
         if acks not in (0, 1, -1, 'all', _missing):
             raise ValueError("Invalid ACKS parameter")
```

### Comparing `aiokafka-0.8.0/aiokafka/producer/sender.py` & `aiokafka-0.8.1/aiokafka/producer/sender.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/producer/transaction_manager.py` & `aiokafka-0.8.1/aiokafka/producer/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/protocol/coordination.py` & `aiokafka-0.8.1/aiokafka/protocol/coordination.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/protocol/transaction.py` & `aiokafka-0.8.1/aiokafka/protocol/transaction.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crc32c.py` & `aiokafka-0.8.1/aiokafka/record/_crc32c.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/consts.pxi` & `aiokafka-0.8.1/aiokafka/record/_crecords/consts.pxi`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/crc32c.c` & `aiokafka-0.8.1/aiokafka/record/_crecords/crc32c.c`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/crc32c.h` & `aiokafka-0.8.1/aiokafka/record/_crecords/crc32c.h`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/cutil.c` & `aiokafka-0.8.1/aiokafka/record/_crecords/cutil.c`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/cutil.pxd` & `aiokafka-0.8.1/aiokafka/record/_crecords/cutil.pxd`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/cutil.pyx` & `aiokafka-0.8.1/aiokafka/record/_crecords/cutil.pyx`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/default_records.c` & `aiokafka-0.8.1/aiokafka/record/_crecords/default_records.c`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/default_records.pxd` & `aiokafka-0.8.1/aiokafka/record/_crecords/default_records.pxd`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/default_records.pyx` & `aiokafka-0.8.1/aiokafka/record/_crecords/default_records.pyx`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/hton.pxd` & `aiokafka-0.8.1/aiokafka/record/_crecords/hton.pxd`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.c` & `aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.c`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.pxd` & `aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.pxd`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/legacy_records.pyx` & `aiokafka-0.8.1/aiokafka/record/_crecords/legacy_records.pyx`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/memory_records.c` & `aiokafka-0.8.1/aiokafka/record/_crecords/memory_records.c`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/_crecords/memory_records.pyx` & `aiokafka-0.8.1/aiokafka/record/_crecords/memory_records.pyx`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/control_record.py` & `aiokafka-0.8.1/aiokafka/record/control_record.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/default_records.py` & `aiokafka-0.8.1/aiokafka/record/default_records.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/legacy_records.py` & `aiokafka-0.8.1/aiokafka/record/legacy_records.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/memory_records.py` & `aiokafka-0.8.1/aiokafka/record/memory_records.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/record/util.py` & `aiokafka-0.8.1/aiokafka/record/util.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/structs.py` & `aiokafka-0.8.1/aiokafka/structs.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka/util.py` & `aiokafka-0.8.1/aiokafka/util.py`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/aiokafka.egg-info/PKG-INFO` & `aiokafka-0.8.1/aiokafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: aiokafka
-Version: 0.8.0
+Version: 0.8.1
 Summary: Kafka integration with asyncio.
 Home-page: http://aiokafka.readthedocs.org
 Download-URL: https://pypi.python.org/pypi/aiokafka
 Author: Andrew Svetlov
 Author-email: andrew.svetlov@gmail.com
 License: Apache 2
 Project-URL: Source, https://github.com/aio-libs/aiokafka
 Platform: POSIX
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Framework :: AsyncIO
 Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: snappy
 Provides-Extra: lz4
 Provides-Extra: zstd
 Provides-Extra: gssapi
 Provides-Extra: all
 License-File: LICENSE
 
@@ -109,15 +108,15 @@
 Docker is required to run tests. See https://docs.docker.com/engine/installation for installation notes. Also note, that `lz4` compression libraries for python will require `python-dev` package,
 or python source header files for compilation on Linux.
 NOTE: You will also need a valid java installation. It's required for the ``keytool`` utility, used to
 generate ssh keys for some tests.
 
 Setting up tests requirements (assuming you're within virtualenv on ubuntu 14.04+)::
 
-    sudo apt-get install -y libsnappy-dev libzstd-dev
+    sudo apt-get install -y libsnappy-dev libzstd-dev libkrb5-dev krb5-user
     make setup
 
 Running tests with coverage::
 
     make cov
 
 To run tests with a specific version of Kafka (default one is 1.0.2) use KAFKA_VERSION variable::
@@ -132,14 +131,36 @@
  * ``make test FLAGS="--no-pull"`` - do not try to pull new docker image before test run.
 
 =========
 Changelog
 =========
 
 
+0.8.1 (2023-05-31)
+==================
+
+New features:
+
+* Drop support for Python 3.7 due to end of life (pr #893)
+
+
+Bugfixes:
+
+* Add SASL authentication support to `AIOKafkaAdminClient` (issue #889,
+  pr #890 by @selevit)
+
+
+Improved Documentation:
+
+* Update `security_protocol` argument docstring (issue #883, pr #884 by
+  @gabrielmbmb)
+* Remove incorrect `await` for `AIOKafkaConsumer.highwater()` (pr #858 by
+  @yi-jiayu)
+
+
 0.8.0 (2022-11-21)
 ==================
 
 New features:
 
 * Add codec for ZStandard compression (KIP-110) (pr #801)
 * Add basic admin client functionality (pr #811 started by @gabriel-tincu)
```

### Comparing `aiokafka-0.8.0/aiokafka.egg-info/SOURCES.txt` & `aiokafka-0.8.1/aiokafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/setup.cfg` & `aiokafka-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiokafka-0.8.0/setup.py` & `aiokafka-0.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,14 @@
             raise RuntimeError("Cannot find version in aiokafka/__init__.py")
 
 
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: System :: Networking",
     "Topic :: System :: Distributed Computing",
@@ -171,15 +170,15 @@
     url="http://aiokafka.readthedocs.org",
     project_urls={
         "Source": "https://github.com/aio-libs/aiokafka",
     },
     download_url="https://pypi.python.org/pypi/aiokafka",
     license="Apache 2",
     packages=["aiokafka"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=install_requires,
     extras_require=extras_require,
     include_package_data=True,
     ext_modules=extensions,
     cmdclass=dict(build_ext=ve_build_ext, bdist_rpm=bdist_rpm),
 )
```

