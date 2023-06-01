# Comparing `tmp/recon_lw-2.0.0.dev5141842548.tar.gz` & `tmp/recon_lw-2.0.0.dev5143256311.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5141842548.tar", last modified: Thu Jun  1 08:03:46 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5143256311.tar", last modified: Thu Jun  1 10:31:59 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5141842548.tar` & `recon_lw-2.0.0.dev5143256311.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 08:03:27.000000 recon_lw-2.0.0.dev5141842548/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33110 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 10:31:39.000000 recon_lw-2.0.0.dev5143256311/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33163 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/LastStateMatcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 from sortedcontainers import SortedKeyList
 from recon_lw import recon_lw
 
 
 class LastStateMatcher:
-    def __init__(self, horizon_delay_seconds, get_timestamp_key1_key2, interpret_func, custom_settings, create_event,
+    def __init__(self, horizon_delay_seconds, get_search_ts_key,
+                 get_state_ts_key_order, interpret_func, custom_settings, create_event,
                  send_events):
-        self._match_index = {}
-        self._time_index = SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0]))
-        self._get_timestamp_key1_key2 = get_timestamp_key1_key2
+        self._search_index = {}
+        self._state_cache = {}
+        self._search_time_index = SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0]))
+        self._state_sequence = {}
+        self._state_time_index = SortedKeyList(key=lambda t: recon_lw.time_stamp_key(t[0]))
+        self._state_cache = {}
+        self._get_search_ts_key = get_search_ts_key
+        self.get_state_ts_key_order = get_state_ts_key_order
         self._interpret_func = interpret_func
         self._create_event = create_event
         self._send_events = send_events
         self._horizon_delay_seconds = horizon_delay_seconds
         self._custom_settings = custom_settings
-        self._debug = True
+        self._debug = False
+
+    def process_objects_batch(self, batch: list) -> None:
+        return
+
+    def flush_all(self) -> None:
+        return
```

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,17 +136,14 @@
                     r["body"]["operation_params"] = initial_parameters
                     r["body"]["initial_book"] = initial_book
                 r["body"]["operation"] = operation.__name__
                 r["body"]["book_id"] = book_id
                 r["parentEventId"] = parent_event["eventId"]
                 r["attachedMessageIds"] = [mess["messageId"]]
                 events.append(r)
-        book["last_operation"] = operation.__name__
-        book["last_params"] = initial_parameters
-
 
     dbg_event = recon_lw.create_event("DebugEvent",
                                       "DebugEvent",
                                       event_sequence,
                                       ok=True,
                                       body={"operations": [(op[0], op[2]["messageId"]) for op in operations_batch],
                                             "len(batch)": len(operations_batch),
@@ -729,20 +726,27 @@
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     ask_unchanged = is_side_unchanged("ask", ask_price, ask_real_qty, ask_impl_qty,
                                       ask_real_n_orders, ask_impl_n_orders, order_book)
-    ask_implied_only = is_side_update_purely_implied("ask", ask_price, ask_real_qty, ask_impl_qty,
-                                                     ask_real_n_orders, ask_impl_n_orders, order_book)
+    if not ask_unchanged:
+        ask_implied_only = is_side_update_purely_implied("ask", ask_price, ask_real_qty, ask_impl_qty,
+                                                         ask_real_n_orders, ask_impl_n_orders, order_book)
+    else:
+        ask_implied_only = False
+
     bid_unchanged = is_side_unchanged("bid", bid_price, bid_real_qty, bid_impl_qty,
                                       bid_real_n_orders, bid_impl_n_orders, order_book)
-    bid_implied_only = is_side_update_purely_implied("bid", bid_price, bid_real_qty, bid_impl_qty,
-                                                     bid_real_n_orders, bid_impl_n_orders, order_book)
+    if not bid_unchanged:
+        bid_implied_only = is_side_update_purely_implied("bid", bid_price, bid_real_qty, bid_impl_qty,
+                                                         bid_real_n_orders, bid_impl_n_orders, order_book)
+    else:
+        bid_implied_only = False
 
     order_book["implied_only"] = (ask_implied_only and bid_unchanged)\
                                  or (bid_implied_only and ask_unchanged) or (bid_implied_only and ask_implied_only)
 
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
```

### Comparing `recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/setup.py` & `recon_lw-2.0.0.dev5143256311/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5141842548/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5143256311/test/test_recon_ob.py`

 * *Files identical despite different names*

