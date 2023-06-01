# Comparing `tmp/blaster-server-0.0.433.tar.gz` & `tmp/blaster-server-0.0.433b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaster-server-0.0.433.tar", last modified: Mon May 29 21:59:39 2023, max compression
+gzip compressed data, was "blaster-server-0.0.433b0.tar", last modified: Thu Jun  1 10:36:25 2023, max compression
```

## Comparing `blaster-server-0.0.433.tar` & `blaster-server-0.0.433b0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1061 2019-07-03 19:03:00.000000 blaster-server-0.0.433/LICENSE.txt
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2022-11-07 18:47:07.000000 blaster-server-0.0.433/MANIFEST.in
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      849 2023-05-29 21:59:39.280180 blaster-server-0.0.433/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2620 2022-11-14 12:45:11.000000 blaster-server-0.0.433/README.md
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2021-10-05 11:27:02.000000 blaster-server-0.0.433/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.276180 blaster-server-0.0.433/blaster/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-01-09 13:10:46.000000 blaster-server-0.0.433/blaster/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.276180 blaster-server-0.0.433/blaster/cloud/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2022-11-09 17:29:08.000000 blaster-server-0.0.433/blaster/cloud/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-29 21:52:39.000000 blaster-server-0.0.433/blaster/cloud/analytics.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.276180 blaster-server-0.0.433/blaster/cloud/aws/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       78 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/cloud/aws/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2022-12-01 11:30:06.000000 blaster-server-0.0.433/blaster/cloud/aws/ses_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-10 23:46:29.000000 blaster-server-0.0.433/blaster/cloud/push_tasks.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-19 10:42:50.000000 blaster-server-0.0.433/blaster/cloud/storage.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3988 2023-05-25 14:24:02.000000 blaster-server-0.0.433/blaster/config.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-01-28 12:57:17.000000 blaster-server-0.0.433/blaster/connection_pool.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       99 2020-11-22 14:37:38.000000 blaster-server-0.0.433/blaster/constants.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5290 2023-05-15 14:09:30.000000 blaster-server-0.0.433/blaster/logging.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62722 2023-05-29 21:57:49.000000 blaster-server-0.0.433/blaster/mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15728 2023-05-17 08:23:45.000000 blaster-server-0.0.433/blaster/schema.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38827 2023-05-25 14:26:32.000000 blaster-server-0.0.433/blaster/server.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    46589 2023-05-22 20:12:00.000000 blaster-server-0.0.433/blaster/tools.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.276180 blaster-server-0.0.433/blaster/utils/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/utils/__init__.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.276180 blaster-server-0.0.433/blaster/utils/data/
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2022-11-08 15:22:07.000000 blaster-server-0.0.433/blaster/utils/data/countries.json
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2022-12-01 10:20:50.000000 blaster-server-0.0.433/blaster/utils/data/mime_types.json
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-14 10:13:13.000000 blaster-server-0.0.433/blaster/utils/data_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-01-07 12:42:21.000000 blaster-server-0.0.433/blaster/utils/events.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-03-30 16:36:26.000000 blaster-server-0.0.433/blaster/utils/fork.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1076 2023-02-21 07:52:48.000000 blaster-server-0.0.433/blaster/utils/lat_long_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-25 14:08:42.000000 blaster-server-0.0.433/blaster/utils/phone_number_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     6773 2020-12-14 07:56:42.000000 blaster-server-0.0.433/blaster/utils/xss_html.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/blaster/websocket/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1022 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12874 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_abnf.py
--rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2022-01-06 11:42:20.000000 blaster-server-0.0.433/blaster/websocket/_app.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    16360 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_core.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     2141 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_exceptions.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     4793 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_handshake.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     7288 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_http.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1870 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_logging.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3623 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_socket.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1550 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_ssl_compat.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3670 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_url.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     3632 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    12758 2021-10-03 12:23:56.000000 blaster-server-0.0.433/blaster/websocket/server.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/blaster/websocket/tests/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/tests/__init__.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)    26115 2019-07-03 19:03:00.000000 blaster-server-0.0.433/blaster/websocket/tests/test_websocket.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/blaster_server.egg-info/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      849 2023-05-29 21:59:39.000000 blaster-server-0.0.433/blaster_server.egg-info/PKG-INFO
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1714 2023-05-29 21:59:39.000000 blaster-server-0.0.433/blaster_server.egg-info/SOURCES.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        1 2023-05-29 21:59:39.000000 blaster-server-0.0.433/blaster_server.egg-info/dependency_links.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      197 2023-05-29 21:59:39.000000 blaster-server-0.0.433/blaster_server.egg-info/requires.txt
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       41 2023-05-29 21:59:39.000000 blaster-server-0.0.433/blaster_server.egg-info/top_level.txt
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/examples/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2019-07-03 19:03:00.000000 blaster-server-0.0.433/examples/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2022-01-06 11:42:20.000000 blaster-server-0.0.433/examples/fast_api_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      636 2019-07-03 19:03:00.000000 blaster-server-0.0.433/examples/gevent_wsgi_test.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      233 2021-10-04 14:48:01.000000 blaster-server-0.0.433/examples/meinheld_flask.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1743 2022-06-17 17:10:40.000000 blaster-server-0.0.433/examples/mongo_ormexample.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2022-11-14 12:13:43.000000 blaster-server-0.0.433/examples/simple_examples.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     1088 2019-07-03 19:03:00.000000 blaster-server-0.0.433/examples/test_chat_room.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      614 2021-02-24 01:34:32.000000 blaster-server-0.0.433/examples/tornado_hello_world.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      791 2021-02-24 01:20:44.000000 blaster-server-0.0.433/examples/wheezy_hello.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)       79 2023-05-29 21:59:39.280180 blaster-server-0.0.433/setup.cfg
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1530 2023-05-29 21:54:00.000000 blaster-server-0.0.433/setup.py
-drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-05-29 21:59:39.280180 blaster-server-0.0.433/test/
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)        0 2022-07-26 21:35:40.000000 blaster-server-0.0.433/test/__init__.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-01-07 00:03:08.000000 blaster-server-0.0.433/test/test_mongo_orm.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-25 13:50:32.000000 blaster-server-0.0.433/test/test_phone_number_utils.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-17 08:26:43.000000 blaster-server-0.0.433/test/test_schema.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)     5457 2022-12-09 21:19:51.000000 blaster-server-0.0.433/test/test_tools.py
--rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-16 18:26:08.000000 blaster-server-0.0.433/test/test_utils.py
--rwxr-xr-x   0 abhinav   (1000) abhinav   (1000)      615 2021-02-24 11:15:27.000000 blaster-server-0.0.433/test/timeit_snippets.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1061 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/LICENSE.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       38 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/MANIFEST.in
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2620 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/README.md
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.846641 blaster-server-0.0.433b0/blaster/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      875 2023-06-01 09:33:08.000000 blaster-server-0.0.433b0/blaster/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.846641 blaster-server-0.0.433b0/blaster/cloud/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       51 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/cloud/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3191 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/cloud/analytics.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.846641 blaster-server-0.0.433b0/blaster/cloud/aws/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       78 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/cloud/aws/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1371 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/cloud/aws/ses_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5221 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/cloud/push_tasks.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5297 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/cloud/storage.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3469 2023-06-01 09:32:59.000000 blaster-server-0.0.433b0/blaster/config.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3715 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/connection_pool.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       99 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/constants.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      772 2023-06-01 09:41:44.000000 blaster-server-0.0.433b0/blaster/env.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5163 2023-06-01 09:29:35.000000 blaster-server-0.0.433b0/blaster/logging.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    62722 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    15727 2023-05-31 09:51:31.000000 blaster-server-0.0.433b0/blaster/schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    38838 2023-05-31 15:34:21.000000 blaster-server-0.0.433b0/blaster/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.846641 blaster-server-0.0.433b0/blaster/tools/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    45886 2023-06-01 09:19:55.000000 blaster-server-0.0.433b0/blaster/tools/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/blaster/utils/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/__init__.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/blaster/utils/data/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)    53078 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/data/countries.json
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)   119011 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/data/mime_types.json
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7085 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/utils/data_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1951 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/events.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     4812 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/fork.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1076 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/lat_long_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     3966 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/blaster/utils/phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6773 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/utils/xss_html.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/blaster/websocket/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1022 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12874 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_abnf.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    11136 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_app.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    16360 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_core.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     2141 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_exceptions.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     4793 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_handshake.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     7288 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_http.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1870 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_logging.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3623 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_socket.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     1550 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_ssl_compat.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3670 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_url.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)     3632 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/_utils.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    12758 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/server.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/blaster/websocket/tests/
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/tests/__init__.py
+-rwxrwxr-x   0 abhinav   (1000) abhinav   (1000)    26115 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/blaster/websocket/tests/test_websocket.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/blaster_server.egg-info/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      851 2023-06-01 10:36:25.000000 blaster-server-0.0.433b0/blaster_server.egg-info/PKG-INFO
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1726 2023-06-01 10:36:25.000000 blaster-server-0.0.433b0/blaster_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        1 2023-06-01 10:36:25.000000 blaster-server-0.0.433b0/blaster_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      197 2023-06-01 10:36:25.000000 blaster-server-0.0.433b0/blaster_server.egg-info/requires.txt
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       41 2023-06-01 10:36:25.000000 blaster-server-0.0.433b0/blaster_server.egg-info/top_level.txt
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/examples/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      266 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/fast_api_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      636 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/gevent_wsgi_test.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      233 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/meinheld_flask.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1743 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/mongo_ormexample.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     2386 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/simple_examples.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1088 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/test_chat_room.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      614 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/tornado_hello_world.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/examples/wheezy_hello.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)       79 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/setup.cfg
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1531 2023-05-31 10:28:22.000000 blaster-server-0.0.433b0/setup.py
+drwxrwxr-x   0 abhinav   (1000) abhinav   (1000)        0 2023-06-01 10:36:25.850641 blaster-server-0.0.433b0/test/
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)        0 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/test/__init__.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     6851 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/test/test_mongo_orm.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      988 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/test/test_phone_number_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     1311 2023-05-30 19:47:55.000000 blaster-server-0.0.433b0/test/test_schema.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)     5457 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/test/test_tools.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      791 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/test/test_utils.py
+-rw-rw-r--   0 abhinav   (1000) abhinav   (1000)      615 2023-04-22 14:53:06.000000 blaster-server-0.0.433b0/test/timeit_snippets.py
```

### Comparing `blaster-server-0.0.433/LICENSE.txt` & `blaster-server-0.0.433b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/PKG-INFO` & `blaster-server-0.0.433b0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.433
+Version: 0.0.433b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.433/README.md` & `blaster-server-0.0.433b0/README.md`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/__init__.py` & `blaster-server-0.0.433b0/blaster/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/cloud/analytics.py` & `blaster-server-0.0.433b0/blaster/cloud/analytics.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/cloud/aws/ses_utils.py` & `blaster-server-0.0.433b0/blaster/cloud/aws/ses_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/cloud/push_tasks.py` & `blaster-server-0.0.433b0/blaster/cloud/push_tasks.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/cloud/storage.py` & `blaster-server-0.0.433b0/blaster/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/config.py` & `blaster-server-0.0.433b0/blaster/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 from os import environ
 import sys
 import os
 import json
-import logging
 import inspect
 # NOTE: don't import anything from blaster library,
 # they may depend on config and won't load correctly.
 # keep it isolated as much as possible
-
-# default env variables
-IS_PROD = environ.get("IS_PROD") == "1"
-IS_STAGING = IS_PROD and environ.get("IS_STAGING") == "1"
-IS_DEV = 1 if not (IS_PROD or IS_STAGING) else 0
-IS_TEST = IS_DEV and environ.get("IS_TEST") == "1"
-
-# CRITICAL-50 ERROR-40  WARNING-30  INFO-20  DEBUG-10  NOTSET-0
-APP_NAME = ""
-APP_VERSION = "0"
-LOG_LEVEL = logging.DEBUG if IS_DEV else (logging.INFO if IS_STAGING else logging.WARN)
-DEBUG_PRINT_LEVEL = IS_DEV and int(environ.get("DEBUG_PRINT_LEVEL") or 0)
-
+from . import env
 
 _this_ = sys.modules[__name__]
 
 
 class Config:
     _config = None
     frozen_keys = None
 
     def __init__(self):
-        self.frozen_keys = {k: v for k, v in vars(_this_).items() if not k.startswith("_")}
+        self.frozen_keys = {k: v for k, v in vars(env).items() if not k.startswith("_")}
         self._config = dict(self.frozen_keys)
 
     def load(self, *paths):
         import yaml
         for path in paths or ["./"]:
             path = os.path.join(
                 os.path.dirname(inspect.stack()[1][1]),  # caller file, called once usually, so no performance impact on app
@@ -98,8 +85,7 @@
 config.BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD = 5000
 
 # MONGO ORM SPECIFIC CONFIGS
 config.MONGO_WARN_MAX_RESULTS_RATE = 1000  # can scan at a max of 1000 / sec
 config.MONGO_MAX_RESULTS_AT_HIGH_SCAN_RATE = 10000  # cannot scan more than this at high scan rate
 config.MONGO_WARN_MAX_QUERY_RESPONSE_TIME_SECONDS = 3  # cannot take more than 3 seconds
 # Logging basics
-config.CONSOLE_LOG_RAW_JSON = False
```

### Comparing `blaster-server-0.0.433/blaster/connection_pool.py` & `blaster-server-0.0.433b0/blaster/connection_pool.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/logging.py` & `blaster-server-0.0.433b0/blaster/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,20 @@
 import time
 from datetime import datetime
 import ujson as json
 from gevent.queue import Queue
 from gevent.threading import Thread
 from logging import DEBUG, INFO, WARN, ERROR
 from .utils import events
-from .config import LOG_LEVEL, APP_VERSION, APP_NAME,\
+from .env import LOG_LEVEL, LOG_APP_NAME, LOG_APP_VERSION,\
 	CONSOLE_LOG_RAW_JSON
 from . import req_ctx
 
 # CRITICAL-50 ERROR-40  WARNING-30  INFO-20  DEBUG-10  NOTSET-0
 
-LOG_APP_NAME = os.getenv("LOG_APP_NAME") or APP_NAME or ""
-LOG_APP_VERSION = os.getenv("LOG_APP_VERSION") or APP_VERSION or ""
-
 _1_DAY_MILLIS = 24 * 60 * 60 * 1000
 _this_ = sys.modules[__name__]
 
 # more levels
 SERVER_INFO = 31
 APP_INFO = 32
 
@@ -139,15 +136,15 @@
 
 	stream_logs_loop.can_run = False
 
 
 @events.register_listener(["blaster_exit1"])
 def flush_and_exit_log_streaming():
 	# don't remove it , it will push an empty function to queues to flush them off
-	LOG(LOG_LEVEL, "log_flushing", msg="flushing logs and exiting")
+	LOG(DEBUG, "log_flushing", msg="flushing logs and exiting")
 
 	log_streaming_thread and log_streaming_thread.join()
 
 
 class PrintColors:
 	HEADER = '\033[95m'
 	OKBLUE = '\033[94m'
```

### Comparing `blaster-server-0.0.433/blaster/mongo_orm.py` & `blaster-server-0.0.433b0/blaster/mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/schema.py` & `blaster-server-0.0.433b0/blaster/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 			})
 
 	@classmethod
 	def from_dict(cls, _dict: dict):
 		ret = cls()
 		for _k, k in cls._dict_key_to_object_key.items():
 			if(_k in _dict):
-				_dict[_k] = _dict.pop(_k)
+				_dict[k] = _dict.pop(_k)
 		cls.validate(_dict, set_obj=ret)
 		return ret
 
 	def to_dict(self):
 		ret = {}
 		for k, attr_validation in self.__class__._validations.items():
 			ret[k] = getattr(self, k, None)
```

### Comparing `blaster-server-0.0.433/blaster/server.py` & `blaster-server-0.0.433b0/blaster/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from . import req_ctx
 from .tools import SanitizedDict,\
 	set_socket_fast_close_options, BufferedSocket, ltrim,\
 	_OBJ_END_
 from .utils import events
 from .utils.data_utils import FILE_EXTENSION_TO_MIME_TYPE
-from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN
+from .logging import LOG_ERROR, LOG_SERVER, LOG_WARN, LOG_DEBUG
 from .schema import Int, Object, Required, schema as schema_func
 from .websocket.server import WebSocketServerHandler
 from .config import IS_DEV, BLASTER_HTTP_TOOK_LONG_WARN_THRESHOLD
 
 if(IS_DEV):
 	# dev specific config
 	from .config import DEV_FORCE_ACCESS_CONTROL_ALLOW_ORIGIN
@@ -1112,17 +1112,18 @@
 			elif(ret == I_AM_HANDLING_THE_SOCKET):
 				close_socket = False
 			break
 
 		if(close_socket):
 			buffered_socket.close()
 
+
 @events.register_listener("blaster_exit0")
 def stop_all_apps():
-	LOG_SERVER("server_info", data="exiting all servers")
+	LOG_DEBUG("server_info", data="exiting all servers")
 	global _is_server_running
 
 	_is_server_running = False
 
 	for app in list(_all_apps):
 		app.stop()  # should handle all connections gracefully
```

### Comparing `blaster-server-0.0.433/blaster/tools.py` & `blaster-server-0.0.433b0/blaster/tools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 @author: abhinav
 '''
 
 from gevent.threading import Thread
 from gevent.queue import Queue
 import os
 import sys
-import subprocess 
+import subprocess
 import shlex
 import collections
 import random
 import string
 import socket
 import struct
 import fcntl
@@ -33,19 +33,19 @@
 import json
 import traceback
 import contextlib
 from io import BytesIO, StringIO
 import requests
 from http.client import HTTPConnection  # py3
 
-from .websocket._core import WebSocket
-from .config import IS_DEV, DEBUG_PRINT_LEVEL
-from .utils.xss_html import XssHtml
-from .utils import events
-from .logging import LOG_APP_INFO, LOG_WARN, LOG_ERROR
+from ..websocket._core import WebSocket
+from ..env import IS_DEV, DEBUG_PRINT_LEVEL
+from ..utils.xss_html import XssHtml
+from ..utils import events
+from ..logging import LOG_APP_INFO, LOG_WARN, LOG_ERROR, LOG_DEBUG
 
 os.environ['TZ'] = 'UTC'
 time.tzset()
 
 # some useful constants
 INT64_MAX = 9223372036854775807
 MILLIS_IN_HOUR = 60 * 60 * 1000
@@ -135,15 +135,15 @@
 
 	def get(self, key, default=None):
 		timestamp_and_value = self.cache.get(key, _OBJ_END_)
 		if(timestamp_and_value == _OBJ_END_):
 			return default
 		if(timestamp_and_value[0] > cur_ms()):
 			return timestamp_and_value[1]
-		self.cache.pop(key, None) # expired object
+		self.cache.pop(key, None)  # expired object
 		return default
 
 	def set(self, key, value):
 		removed_entries = []
 		cur_timestamp = cur_ms()
 		while(len(self.cache) >= self.capacity):
 			removed_entries.append(self.cache.popitem(last=False))
@@ -1642,45 +1642,20 @@
 	pass
 
 
 # when server shutsdown
 _joinables = []
 
 
-# Background tasks START
-
-def __background_tasks_runner_thread(func, args=(), kwargs={}):
-	if(not __background_tasks_runner_thread.can_run_tasks):
-		LOG_WARN(
-			"background_threads",
-			msg="Cannot run background threads. Correct copepaths"
-		)
-		return
-
-	LOG_APP_INFO(
-		"background_threads", msg="starting background thread",
-		func=func.__name__
-	)
-	_thread_to_start = Thread(
-		target=func,
-		args=args,
-		kwargs=kwargs
-	)
-	_joinables.append(_thread_to_start)
-	_thread_to_start.start()
-
-
-__background_tasks_runner_thread.can_run_tasks = True
-
 # partioned queues
 _partitioned_background_task_queues = tuple(Queue() for _ in range(4))
 
 
-def _process_partitioned_task_queue_items(_queue):
-	while __background_tasks_runner_thread.can_run_tasks or not _queue.empty():
+def _process_task_queue(_queue):
+	while _process_task_queue.can_process or not _queue.empty():
 		func, args, kwargs = _queue.get()
 		_start_time = time.time()
 		try:
 			func(*args, **kwargs)
 		except Exception as ex:
 			stacktrace_string = traceback.format_exc()
 			LOG_ERROR(
@@ -1696,84 +1671,78 @@
 			LOG_WARN(
 				"background_task_perf",
 				func_name=func.__name__,
 				elapsed_millis=int(_elapsed_time * 1000),
 			)
 
 
+_process_task_queue.can_process = True
+_process_task_queue._background_thread_started = False
 # singleton
-def __start_task_processors():
-	# start threads to process entries in partitioned queues
-	for _queue in _partitioned_background_task_queues:
-		__background_tasks_runner_thread(
-			_process_partitioned_task_queue_items, args=(_queue,)
-		)
-	__start_task_processors.started = True
-
-
-# set initial flag
-__start_task_processors.started = False
 
 
 # submit a task:func to a partition
 # parition is used when you want them to execute in the
 # same order as submitted
 def submit_background_task(partition_key, func, *args, **kwargs):
 	# start processors if not started already
-	if(not __start_task_processors.started):
-		__start_task_processors()
-
 	if(partition_key == None):
 		partition_key = cur_ms()  # choose a random key
-	_partitioned_background_task_queues[hash(str(partition_key)) % len(_partitioned_background_task_queues)]\
-		.put((func, args, kwargs))
+	_queue = _partitioned_background_task_queues[hash(str(partition_key)) % len(_partitioned_background_task_queues)]
+
+	if(not _process_task_queue.can_process):
+		raise Exception("Cannot submit tasks to a queue which is not processing")
+
+	if(not _process_task_queue._background_thread_started):
+		_process_task_queue._background_thread_started = True
+		_thread_to_start = Thread(
+			target=_process_task_queue,
+			args=(_queue,),
+		)
+		_joinables.append(_thread_to_start)
+		LOG_APP_INFO(
+			"background_threads", msg="starting background tasks processor thread",
+			func=_process_task_queue.__name__
+		)
+		_thread_to_start.start()
+	_queue.put((func, args, kwargs))
 
 
 # decorator to be used for a short io tasks to be
 # run in background
 def background_task(func):
 	def wrapper(*args, **kwargs):
 		# spawn the thread
-		if(not __background_tasks_runner_thread.can_run_tasks):
-			LOG_WARN(
-				"background_threads",
-				msg="Cannot run background threads as can_run flag is not set. Correct codepaths"
-			)
-			return
 		submit_background_task(None, func, *args, **kwargs)
 		return True
 
 	wrapper._original = getattr(func, "_original", func)
 	return wrapper
 
 
 # Blaster exit functions
 @events.register_listener(["blaster_exit0"])
 def exit_0():
 	# start of exit - background threads cannot run
-	if(not __background_tasks_runner_thread.can_run_tasks):
-		return  # double calling function
-
-	__background_tasks_runner_thread.can_run_tasks = False
-
 	# push an empty function to queues to flush them off
-	for _partitioned_task_queue in _partitioned_background_task_queues:
-		_partitioned_task_queue.put((empty_func, [], {}))
+	_process_task_queue.can_process = False
+	for _queue in _partitioned_background_task_queues:
+		_queue.put((empty_func, [], {}))
 
 # Background tasks END
 
 
 @events.register_listener(["blaster_exit5"])
 def exit_5():
 	# reap all joinables of background threads,
 	# everything should be done by this point
 	for _joinable in _joinables:
 		_joinable.join()
 	_joinables.clear()
-	LOG_APP_INFO("background_threads", msg="cleanedup")
+	LOG_DEBUG("background_threads", msg="cleanedup")
 
 
 # calls a function after the function returns given by argument after
 def call_after_func(func):
 
 	if(isinstance(func, str)):
 		# after_func => take from args named by func
```

### Comparing `blaster-server-0.0.433/blaster/utils/data/countries.json` & `blaster-server-0.0.433b0/blaster/utils/data/countries.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/data/mime_types.json` & `blaster-server-0.0.433b0/blaster/utils/data/mime_types.json`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/data_utils.py` & `blaster-server-0.0.433b0/blaster/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/events.py` & `blaster-server-0.0.433b0/blaster/utils/events.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/fork.py` & `blaster-server-0.0.433b0/blaster/utils/fork.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/lat_long_utils.py` & `blaster-server-0.0.433b0/blaster/utils/lat_long_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/phone_number_utils.py` & `blaster-server-0.0.433b0/blaster/utils/phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/utils/xss_html.py` & `blaster-server-0.0.433b0/blaster/utils/xss_html.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/__init__.py` & `blaster-server-0.0.433b0/blaster/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_abnf.py` & `blaster-server-0.0.433b0/blaster/websocket/_abnf.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_app.py` & `blaster-server-0.0.433b0/blaster/websocket/_app.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_core.py` & `blaster-server-0.0.433b0/blaster/websocket/_core.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_exceptions.py` & `blaster-server-0.0.433b0/blaster/websocket/_exceptions.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_handshake.py` & `blaster-server-0.0.433b0/blaster/websocket/_handshake.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_http.py` & `blaster-server-0.0.433b0/blaster/websocket/_http.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_logging.py` & `blaster-server-0.0.433b0/blaster/websocket/_logging.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_socket.py` & `blaster-server-0.0.433b0/blaster/websocket/_socket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_ssl_compat.py` & `blaster-server-0.0.433b0/blaster/websocket/_ssl_compat.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_url.py` & `blaster-server-0.0.433b0/blaster/websocket/_url.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/_utils.py` & `blaster-server-0.0.433b0/blaster/websocket/_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/server.py` & `blaster-server-0.0.433b0/blaster/websocket/server.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster/websocket/tests/test_websocket.py` & `blaster-server-0.0.433b0/blaster/websocket/tests/test_websocket.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/blaster_server.egg-info/PKG-INFO` & `blaster-server-0.0.433b0/blaster_server.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blaster-server
-Version: 0.0.433
+Version: 0.0.433b0
 Summary: Gevent based python server built from scratch for maximum performance
 Home-page: https://github.com/abhinavabcd/blaster
 Author: Abhinav Reddy
 Author-email: abhinavabcd@gmail.com
 License: MIT
 Download-URL: https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz
 Keywords: server,superfast,Like FastApi or Flask but 10x faster
```

### Comparing `blaster-server-0.0.433/blaster_server.egg-info/SOURCES.txt` & `blaster-server-0.0.433b0/blaster_server.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-__init__.py
 setup.cfg
 setup.py
 blaster/__init__.py
 blaster/config.py
 blaster/connection_pool.py
 blaster/constants.py
+blaster/env.py
 blaster/logging.py
 blaster/mongo_orm.py
 blaster/schema.py
 blaster/server.py
-blaster/tools.py
 blaster/cloud/__init__.py
 blaster/cloud/analytics.py
 blaster/cloud/push_tasks.py
 blaster/cloud/storage.py
 blaster/cloud/aws/__init__.py
 blaster/cloud/aws/ses_utils.py
+blaster/tools/__init__.py
 blaster/utils/__init__.py
 blaster/utils/data_utils.py
 blaster/utils/events.py
 blaster/utils/fork.py
 blaster/utils/lat_long_utils.py
 blaster/utils/phone_number_utils.py
 blaster/utils/xss_html.py
```

### Comparing `blaster-server-0.0.433/examples/gevent_wsgi_test.py` & `blaster-server-0.0.433b0/examples/gevent_wsgi_test.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/examples/mongo_ormexample.py` & `blaster-server-0.0.433b0/examples/mongo_ormexample.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/examples/simple_examples.py` & `blaster-server-0.0.433b0/examples/simple_examples.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/examples/test_chat_room.py` & `blaster-server-0.0.433b0/examples/test_chat_room.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/examples/tornado_hello_world.py` & `blaster-server-0.0.433b0/examples/tornado_hello_world.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/examples/wheezy_hello.py` & `blaster-server-0.0.433b0/examples/wheezy_hello.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/setup.py` & `blaster-server-0.0.433b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
 	name='blaster-server',
 	packages=find_packages() + ["blaster/utils/data"],
-	version='0.0.433',
+	version='0.0.433b',
 	license='MIT',
 	description='Gevent based python server built from scratch for maximum performance',
 	author='Abhinav Reddy',                   # Type in your name
 	author_email='abhinavabcd@gmail.com',      # Type in your E-Mail
 	url='https://github.com/abhinavabcd/blaster',
 	download_url='https://github.com/abhinavabcd/blaster/archive/v0.0337b.tar.gz',
 	keywords=['server', 'superfast', 'Like FastApi or Flask but 10x faster'],
 	include_package_data=True,
 	install_requires=[            # I get to this in a second
 		"wheel>=0.34.2",
 		"pytz>=2020.1",
-		"gevent>=20.9.0",
+		"gevent>=22.9.0",
 		"greenlet>=2.0.1",
 		"pymongo>=3.12.0",
 		"ujson>=2.0.3",
 		"python-dateutil>=2.8.1",
 		"requests>=2.25.1",
 		"requests-toolbelt>=0.9.1",
 		"urllib3>=1.26.4",
```

### Comparing `blaster-server-0.0.433/test/test_mongo_orm.py` & `blaster-server-0.0.433b0/test/test_mongo_orm.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/test/test_phone_number_utils.py` & `blaster-server-0.0.433b0/test/test_phone_number_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/test/test_schema.py` & `blaster-server-0.0.433b0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/test/test_tools.py` & `blaster-server-0.0.433b0/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/test/test_utils.py` & `blaster-server-0.0.433b0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `blaster-server-0.0.433/test/timeit_snippets.py` & `blaster-server-0.0.433b0/test/timeit_snippets.py`

 * *Files identical despite different names*

