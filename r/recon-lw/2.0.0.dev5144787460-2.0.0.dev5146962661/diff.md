# Comparing `tmp/recon_lw-2.0.0.dev5144787460.tar.gz` & `tmp/recon_lw-2.0.0.dev5146962661.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5144787460.tar", last modified: Thu Jun  1 13:13:33 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5146962661.tar", last modified: Thu Jun  1 16:42:39 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5144787460.tar` & `recon_lw-2.0.0.dev5146962661.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 13:13:15.000000 recon_lw-2.0.0.dev5144787460/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33387 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22339 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 16:42:21.000000 recon_lw-2.0.0.dev5146962661/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32712 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22337 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 16:42:39.000000 recon_lw-2.0.0.dev5146962661/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 16:41:58.000000 recon_lw-2.0.0.dev5146962661/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/recon_ob.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,19 @@
     events.append(debug_event)
 
     for operation, parameters, mess in operations_batch:
         initial_book = copy.deepcopy(book)
         initial_parameters = copy.copy(parameters)
         parameters["order_book"] = book
         result, log_entries = operation(**parameters)
+        if "v" not in book:
+            book["v"] = 1
+        else:
+            book["v"] += 1
+
         if len(result) > 0:
             result["operation"] = operation.__name__
             result["operation_params"] = initial_parameters
             result["initial_book"] = initial_book
             result["book_id"] = book_id
             update_event = recon_lw.create_event("UpdateBookError:" + parent_event["eventName"], "UpdateBookError",
                                                  event_sequence,
@@ -162,24 +167,36 @@
             if obs[i]["operation"] in ["ob_change_status", "ob_clean_book", "ob_aggr_clean_book", "ob_top_clean_book"]:
                 obs[i]["aggr_seq"]["top_v2"] = updated_v2
                 obs[i]["aggr_seq"]["limit_v2"] = updated_v2
                 updated_v2 += 1
                 continue
 
             obs[i]["aggr_seq"]["top_delta"] = 0
-            obs[i]["aggr_seq"]["top_v"] = -1
             obs[i]["aggr_seq"]["top_v2"] = -1
             obs[i]["aggr_seq"]["limit_delta"] = 0
-            obs[i]["aggr_seq"]["limit_v"] = -1
             obs[i]["aggr_seq"]["limit_v2"] = -1
 
         obs[-1]["aggr_seq"]["top_delta"] = 0 if top_not_affected else 1
         obs[-1]["aggr_seq"]["top_v2"] = updated_v2
         obs[-1]["aggr_seq"]["limit_delta"] = 0 if limit_not_affected else 1
         obs[-1]["aggr_seq"]["limit_v2"] = updated_v2
+    else:
+        updated_limit_v2 = 0
+        updated_top_v2 = 0
+        for i in range(len(obs)):
+            if obs[i]["aggr_seq"]["top_delta"] == 1:
+                obs[i]["aggr_seq"]["top_v2"] = updated_top_v2
+                updated_top_v2 += 1
+            else:
+                obs[i]["aggr_seq"]["top_v2"] = -1
+            if obs[i]["aggr_seq"]["limit_delta"] == 1:
+                obs[i]["aggr_seq"]["limit_v2"] = updated_limit_v2
+                updated_limit_v2 += 1
+            else:
+                obs[i]["aggr_seq"]["limit_v2"] = -1
 
 
 def process_market_data_update(mess_batch, events,  books_cache, get_book_id_func ,update_book_rule,
                                check_book_rule, event_sequence, parent_event, initial_book_params, log_books_filter,
                                log_books_collection, aggregate_batch_updates):
     books_updates = {}
     for m in mess_batch:
@@ -306,56 +323,57 @@
         dupl_events.append(d_ev)
     save_events_func(dupl_events)
     duplicates.clear()
     flush_sequence_clear_cache(n_processed, rule_settings["sequence_cache"])
 
 
 def init_aggr_seq(order_book: dict) -> None:
-    order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0, "limit_v2" : 0, "top_v2" : 0, "affected_side": "na", "affected_level": -1}
+    #order_book["aggr_seq"] = {"top_v": 0, "top_delta": 0, "limit_v": 0, "limit_delta": 0, "limit_v2" : 0, "top_v2" : 0, "affected_side": "na", "affected_level": -1}
+    order_book["aggr_seq"] = {"top_delta": 0, "limit_delta": 0}
     order_book["implied_only"] = False
 
 
 def reset_aggr_seq(order_book):
-    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0, "affected_side": "na", "affected_level": -1})
+    order_book["aggr_seq"].update({"top_delta": 0, "limit_delta": 0})
     order_book["implied_only"] = False
 
 
 def reflect_price_update_in_version(side: str, price: float,str_time_of_event,order_book: dict):
     level = get_price_level(side, price, order_book)
-    order_book["aggr_seq"]["affected_side"] = side
-    order_book["aggr_seq"]["affected_level"] = level
+    #order_book["aggr_seq"]["affected_side"] = side
+    #order_book["aggr_seq"]["affected_level"] = level
 
     max_levels = order_book["aggr_max_levels"]
     if level <= max_levels:
-        order_book["aggr_seq"]["limit_v"] += 1
+        #order_book["aggr_seq"]["limit_v"] += 1
         order_book["aggr_seq"]["limit_delta"] = 1
     if level == 1:
-        order_book["aggr_seq"]["top_v"] += 1
+        #order_book["aggr_seq"]["top_v"] += 1
         order_book["aggr_seq"]["top_delta"] = 1
 
     if "time_of_event" not in order_book:
         order_book["time_of_event"] = str_time_of_event
-        order_book["aggr_seq"]["limit_v2"] = 0
-        order_book["aggr_seq"]["limit_v2"] = 0
-    else:
-        if str_time_of_event == order_book["time_of_event"]:
-            if level <= max_levels:
-                order_book["aggr_seq"]["limit_v2"] += 1
-            if level == 1:
-                order_book["aggr_seq"]["top_v2"] += 1
-        else:
-            order_book["time_of_event"] = str_time_of_event
-            if level <= max_levels:
-                order_book["aggr_seq"]["limit_v2"] = 0
-            else:
-                order_book["aggr_seq"]["limit_v2"] = -1
-            if level == 1:
-                order_book["aggr_seq"]["top_v2"] = 0
-            else:
-                order_book["aggr_seq"]["top_v2"] = -1
+        #order_book["aggr_seq"]["limit_v2"] = 0
+        #order_book["aggr_seq"]["limit_v2"] = 0
+    #else:
+    #    if str_time_of_event == order_book["time_of_event"]:
+    #        if level <= max_levels:
+    #            order_book["aggr_seq"]["limit_v2"] += 1
+    #        if level == 1:
+    #            order_book["aggr_seq"]["top_v2"] += 1
+    #    else:
+     #       order_book["time_of_event"] = str_time_of_event
+     #       if level <= max_levels:
+     #           order_book["aggr_seq"]["limit_v2"] = 0
+     #       else:
+     #           order_book["aggr_seq"]["limit_v2"] = -1
+     #       if level == 1:
+     #           order_book["aggr_seq"]["top_v2"] = 0
+     #       else:
+     #           order_book["aggr_seq"]["top_v2"] = -1
 
 
 def ob_add_order(order_id: str, price: float, size: int, side: str, str_time_of_event ,order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
@@ -415,21 +433,14 @@
     log = []
     reflect_price_update_in_version(old_side, old_price,str_time_of_event,order_book)
     order_book[old_side][old_price].pop(order_id)
     if len(order_book[old_side][old_price]) == 0:
         order_book[old_side].pop(old_price)
         log.append(copy.deepcopy(order_book))
         max_levels = order_book["aggr_max_levels"]
-        if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
-            # back from horizon update
-            order_book["aggr_seq"]["limit_delta"] = 2
-            order_book["aggr_seq"]["limit_v"] += 1
-            order_book["aggr_seq"]["limit_v2"] += 1
-
-            log.append(copy.deepcopy(order_book))
     else:
         log.append(copy.deepcopy(order_book))
 
     return {}, log
 
 
 def ob_trade_order(order_id: str, traded_size: int, str_time_of_event, order_book: dict) -> tuple:
@@ -446,21 +457,14 @@
         return {"error": "traded size > resting size"}, []
     elif traded_size == old_size:
         reflect_price_update_in_version(old_side, old_price, str_time_of_event,order_book)
         order_book[old_side][old_price].pop(order_id)
         if len(order_book[old_side][old_price]) == 0:
             order_book[old_side].pop(old_price)
             log.append(copy.deepcopy(order_book))
-            max_levels = order_book["aggr_max_levels"]
-            if len(order_book[old_side]) >= max_levels and order_book["aggr_seq"]["limit_delta"] == 1:
-                # back from horizon update
-                order_book["aggr_seq"]["limit_delta"] = 2
-                order_book["aggr_seq"]["limit_v"] += 1
-                order_book["aggr_seq"]["limit_v2"] += 1
-                log.append(copy.deepcopy(order_book))
         else:
             log.append(copy.deepcopy(order_book))
     else:
         reflect_price_update_in_version(old_side, old_price, str_time_of_event ,order_book)
         order_book[old_side][old_price][order_id] -= traded_size
         log.append(copy.deepcopy(order_book))
     return {}, log
@@ -474,33 +478,29 @@
 
     for side_key in ["ask", "bid"]:
         if side_key in order_book:
             order_book[side_key].clear()
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
-    order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_change_status(new_status: str, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
     order_book["status"] = new_status
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
     order_book["aggr_seq"]["top_delta"] = 1
-    order_book["aggr_seq"]["top_v"] += 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def find_order_position(order_id: str, order_book: dict) -> tuple:
     for side in ["ask", "bid"]:
         for pr, orders in order_book[side].items():
             if order_id in orders:
@@ -516,23 +516,16 @@
     levels.sort()
     return levels.index(p) + 1 if side == "ask" else len(levels) - levels.index(p)
 
 
 def update_time_and_version(str_time_of_event, order_book):
     if "time_of_event" not in order_book:
         order_book["time_of_event"] = str_time_of_event
-        order_book["aggr_seq"]["limit_v2"] = 0
-        order_book["aggr_seq"]["top_v2"] = 0
     else:
-        if str_time_of_event == order_book["time_of_event"]:
-            order_book["aggr_seq"]["limit_v2"] += 1
-            order_book["aggr_seq"]["top_v2"] += 1
-        else:
-            order_book["aggr_seq"]["limit_v2"] = 0
-            order_book["aggr_seq"]["top_v2"] = 0
+        if str_time_of_event != order_book["time_of_event"]:
             order_book["time_of_event"] = str_time_of_event
 
 
 def ob_aggr_add_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
                       impl_num_orders: int, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
@@ -552,17 +545,18 @@
 
     new_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders, "impl_qty": impl_qty,
                  "impl_num_orders": impl_num_orders}
     order_book[side_key].insert(new_index, new_level)
     if len(order_book[side_key]) == max_levels + 1:
         order_book[side_key].pop()
 
+    order_book["aggr_seq"]["top_delta"] = (new_index == 0)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
+
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_delete_level(side: str, level: int, str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
@@ -576,17 +570,18 @@
         return result_body, []
 
     #is it purely implied
     order_book["implied_only"] = (order_book[side_key][del_index]["real_num_orders"] == 0)
 
     order_book[side_key].pop(del_index)
 
+    order_book["aggr_seq"]["top_delta"] = (del_index == 0)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
+
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_update_level(side: str, level: int, price: float, real_qty: int, real_num_orders: int, impl_qty: int,
                          impl_num_orders: int,
                          str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
@@ -606,17 +601,18 @@
     order_book["implied_only"] = (order_book[side_key][update_index]["real_num_orders"] == real_num_orders) and \
                                  (order_book[side_key][update_index]["real_qty"] == real_qty)
 
 
     upd_level = {"price": price, "real_qty": real_qty, "real_num_orders": real_num_orders,
                  "impl_qty": impl_qty, "impl_num_orders": impl_num_orders}
     order_book[side_key][update_index].update(upd_level)
+
+    order_book["aggr_seq"]["top_delta"] = (update_index == 0)
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_aggr_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
@@ -624,15 +620,15 @@
         reset_aggr_seq(order_book)
 
     for side_key in ["ask_aggr", "bid_aggr"]:
         if side_key in order_book:
             order_book[side_key].clear()
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["limit_delta"] = 1
-    order_book["aggr_seq"]["limit_v"] += 1
+    order_book["aggr_seq"]["top_delta"] = 1
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_top_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
@@ -647,15 +643,14 @@
     order_book["bid_real_qty"] = 0
     order_book["bid_impl_qty"] = 0
     order_book["bid_real_n_orders"] = 0
     order_book["bid_impl_n_orders"] = 0
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
-    order_book["aggr_seq"]["top_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
 
 
 def ob_indicative_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
@@ -710,15 +705,15 @@
     reverse = -1 if side == "bid" else 1
     if new_price is None:  # deleted level
         return book[side+"_real_n_orders"] == 0
     elif book[side+"_price"] is None:  # added level to empty book
         return new_real_n_orders == 0
     if book[side+"_price"] == new_price:  # top level update
         return new_real_n_orders == book[side+"_real_n_orders"] and book[side+"_real_qty"] == new_real_qty
-    if reverse * book[side+"_price"] < reverse * new_price:  # price is better - new level is added
+    if (reverse * book[side+"_price"]) < (reverse * new_price):  # price is better - new level is added
         return new_real_n_orders == 0
     else:  # price is worse old level is deleted
         return book[side+"_real_n_orders"] == 0
 
 
 def ob_top_update(ask_price: float, ask_real_qty: int, ask_impl_qty: int, ask_real_n_orders: int, ask_impl_n_orders: int,
                   bid_price: float, bid_real_qty: int, bid_impl_qty: int, bid_real_n_orders: int, bid_impl_n_orders: int,
@@ -762,10 +757,9 @@
     order_book["bid_real_qty"] = bid_real_qty
     order_book["bid_impl_qty"] = bid_impl_qty
     order_book["bid_real_n_orders"] = bid_real_n_orders
     order_book["bid_impl_n_orders"] = bid_impl_n_orders
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
-    order_book["aggr_seq"]["top_v"] += 1
 
     return {}, [copy.deepcopy(order_book)]
```

### Comparing `recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5146962661/recon_lw/recon_ob_cross_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                             o["body"]["time_of_event"],
                                                             o["body"]["aggr_seq"]["top_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["aggr_session"]:
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
-                                                                  o["body"]["aggr_seq"]["limit_v2"])
+                                                                  o["body"]["aggr_seq"]["top_v2"])
 
     return None, None, None
 
 
 def ob_compare_interpret_match_aggr(match, custom_settings, create_event, save_events):
     if match[0] is not None and match[1] is not None:
         comp_res = compare_full_vs_aggr(match[0]["body"], match[1]["body"])
```

### Comparing `recon_lw-2.0.0.dev5144787460/setup.py` & `recon_lw-2.0.0.dev5146962661/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144787460/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5146962661/test/test_recon_ob.py`

 * *Files identical despite different names*

