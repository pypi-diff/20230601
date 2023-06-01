# Comparing `tmp/recon_lw-2.0.0.dev5144147090.tar.gz` & `tmp/recon_lw-2.0.0.dev5144787460.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5144147090.tar", last modified: Thu Jun  1 12:13:14 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5144787460.tar", last modified: Thu Jun  1 13:13:33 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5144147090.tar` & `recon_lw-2.0.0.dev5144787460.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 12:12:50.000000 recon_lw-2.0.0.dev5144147090/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33169 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 13:13:15.000000 recon_lw-2.0.0.dev5144787460/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33387 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22339 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 13:13:33.000000 recon_lw-2.0.0.dev5144787460/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 13:12:53.000000 recon_lw-2.0.0.dev5144787460/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,14 +740,20 @@
                                       bid_real_n_orders, bid_impl_n_orders, order_book)
     if not bid_unchanged:
         bid_implied_only = is_side_update_purely_implied("bid", bid_price, bid_real_qty, bid_impl_qty,
                                                          bid_real_n_orders, bid_impl_n_orders, order_book)
     else:
         bid_implied_only = False
 
+    order_book["implied_only_debug"] = {
+        "ask_unchanged": ask_unchanged,
+        "ask_implied_only": ask_implied_only,
+        "bid_unchanged": bid_unchanged,
+        "bid_implied_only": bid_implied_only
+    }
     order_book["implied_only"] = (ask_implied_only and bid_unchanged)\
                                  or (bid_implied_only and ask_unchanged) or (bid_implied_only and ask_implied_only)
 
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
```

### Comparing `recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5144787460/recon_lw/recon_ob_cross_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
         if top_book["bid_real_qty"] != 0 or top_book["bid_impl_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "bid"})
     return problems
 
 
 def compare_full_vs_top(full_book: dict, top_book: dict):
     problems = []
-    if len(full_book["ask"]) > 0:
+    if top_book["ask_real_n_orders"] == 0 and top_book["ask_impl_n_orders"] != 0:
+        problems = []
+    elif len(full_book["ask"]) > 0:
         if top_book["ask_real_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "ask"})
         else:
             top_p = min(full_book["ask"].keys())
             price_condition = top_p == top_book["ask_price"]
             num_orders_condition = len(full_book["ask"][top_p]) == \
                                    (top_book["ask_real_n_orders"])
@@ -108,15 +110,17 @@
             if not (price_condition and num_orders_condition and size_condition):
                 problems.append({"synopsys": synopsys(price_condition, num_orders_condition, size_condition),
                                  "side": "ask"})
     else:
         if top_book["ask_real_qty"] != 0:
             problems.append({"synopsys": "full_miss_level", "side": "ask"})
 
-    if len(full_book["bid"]) > 0:
+    if top_book["bid_real_n_orders"] == 0 and top_book["bid_impl_n_orders"] != 0:
+        problems = problems
+    elif len(full_book["bid"]) > 0:
         if top_book["bid_real_qty"] == 0:
             problems.append({"synopsys": "top_miss_level", "side": "bid"})
         else:
             top_p = max(full_book["bid"].keys())
             price_condition = top_p == top_book["bid_price"]
             num_orders_condition = len(full_book["bid"][top_p]) == \
                                    (top_book["bid_real_n_orders"])
@@ -135,16 +139,14 @@
         return None, None, None
     if o["body"]["sessionId"] == custom_settings["full_session"]:
         return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                             o["body"]["time_of_event"],
                                                             o["body"]["aggr_seq"]["limit_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
-        if "implied_only" in o["body"] and o["body"]["implied_only"]:
-            return None, None, None
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
                                                                   o["body"]["aggr_seq"]["limit_v2"])
 
     return None, None, None
 
 
@@ -154,16 +156,14 @@
 
     if o["body"]["sessionId"] == custom_settings["full_session"]:
         return o["body"]["timestamp"], "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                             o["body"]["time_of_event"],
                                                             o["body"]["aggr_seq"]["top_v2"]), None
 
     if o["body"]["sessionId"] == custom_settings["comp_session"]:
-        if "implied_only" in o["body"] and o["body"]["implied_only"]:
-            return None, None, None
         return o["body"]["timestamp"], None, "{0}_{1}_{2}".format(o["body"]["book_id"],
                                                                   o["body"]["time_of_event"],
                                                                   o["body"]["aggr_seq"]["top_v2"])
 
     return None, None, None
 
 
@@ -207,16 +207,17 @@
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "limit_v2": match[0]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[0]["body"]["sessionId"],
                                     "tech_info": tech_info})
         save_events([error_event])
     elif match[1] is not None:
-        error_event = create_event("StreamMismatchNoFullvsAggr",
-                                   "StreamMismatchNoFullvsAggr",
+        e_type = "StreamMismatchNoFullvsAggrImpl" if match[1]["body"]["implied_only"] else "StreamMismatchNoFullvsAggr"
+        error_event = create_event(e_type,
+                                   e_type,
                                    False,
                                    {"aggr_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                    "limit_v2": match[1]["body"]["aggr_seq"]["limit_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
@@ -243,16 +244,17 @@
                                    {"full_book_event": match[0]["eventId"],
                                     "book_id": match[0]["body"]["book_id"],
                                     "time_of_event": match[0]["body"]["time_of_event"],
                                     "top_v2": match[0]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[0]["body"]["sessionId"]})
         save_events([error_event])
     elif match[1] is not None:
-        error_event = create_event("StreamMismatchNoFullvsTop",
-                                   "StreamMismatchNoFullvsTop",
+        e_type = "StreamMismatchNoFullvsTopImpl" if match[1]["body"]["implied_only"] else "StreamMismatchNoFullvsTop"
+        error_event = create_event(e_type,
+                                   e_type,
                                    False,
                                    {"top_book_event": match[1]["eventId"],
                                     "book_id": match[1]["body"]["book_id"],
                                     "time_of_event": match[1]["body"]["time_of_event"],
                                     "top_v2": match[1]["body"]["aggr_seq"]["top_v2"],
                                     "sessionId": match[1]["body"]["sessionId"]})
         save_events([error_event])
```

### Comparing `recon_lw-2.0.0.dev5144147090/setup.py` & `recon_lw-2.0.0.dev5144787460/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5144147090/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5144787460/test/test_recon_ob.py`

 * *Files identical despite different names*

