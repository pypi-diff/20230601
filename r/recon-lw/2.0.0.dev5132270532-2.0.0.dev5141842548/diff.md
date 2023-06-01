# Comparing `tmp/recon_lw-2.0.0.dev5132270532.tar.gz` & `tmp/recon_lw-2.0.0.dev5141842548.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5132270532.tar", last modified: Wed May 31 11:29:16 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5141842548.tar", last modified: Thu Jun  1 08:03:46 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5132270532.tar` & `recon_lw-2.0.0.dev5141842548.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-31 11:28:55.000000 recon_lw-2.0.0.dev5132270532/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)      692 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32005 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:29:16.000000 recon_lw-2.0.0.dev5132270532/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-05-31 11:28:32.000000 recon_lw-2.0.0.dev5132270532/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 08:03:27.000000 recon_lw-2.0.0.dev5141842548/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)      692 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33110 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 08:03:46.000000 recon_lw-2.0.0.dev5141842548/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 08:03:02.000000 recon_lw-2.0.0.dev5141842548/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob.py`

 * *Files 2% similar despite different names*

```diff
@@ -692,49 +692,60 @@
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 0
     order_book["aggr_seq"]["limit_delta"] = 0
 
     return {}, [copy.deepcopy(order_book)]
 
 
+def is_side_unchanged(side, new_price, new_real_qty, new_impl_qty, new_real_n_orders, new_impl_n_orders, book):
+    if new_price is None:
+        return book[side+"_price"] is None
+    if book[side+"_price"] is None:
+        return False
+    return book[side+"_price"] == new_price and \
+           book[side+"_real_qty"] == new_real_qty and \
+           book[side+"_impl_qty"] == new_impl_qty and \
+           book[side+"_real_n_orders"] == new_real_n_orders and \
+           book[side+"_impl_n_orders"] == new_impl_n_orders
+
+
+def is_side_update_purely_implied(side, new_price, new_real_qty, new_impl_qty,
+                                  new_real_n_orders, new_impl_n_orders, book):
+    reverse = -1 if side == "bid" else 1
+    if new_price is None:  # deleted level
+        return book[side+"_real_n_orders"] == 0
+    elif book[side+"_price"] is None:  # added level to empty book
+        return new_real_n_orders == 0
+    if book[side+"_price"] == new_price:  # top level update
+        return new_real_n_orders == book[side+"_real_n_orders"] and book[side+"_real_qty"] == new_real_qty
+    if reverse * book[side+"_price"] < reverse * new_price:  # price is better - new level is added
+        return new_real_n_orders == 0
+    else:  # price is worse old level is deleted
+        return book[side+"_real_n_orders"] == 0
+
+
 def ob_top_update(ask_price: float, ask_real_qty: int, ask_impl_qty: int, ask_real_n_orders: int, ask_impl_n_orders: int,
                   bid_price: float, bid_real_qty: int, bid_impl_qty: int, bid_real_n_orders: int, bid_impl_n_orders: int,
                   str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
-    #is it purely implied
-    sell_implieds_only = False
-    if ask_price == order_book["ask_price"]:
-        if ask_real_n_orders == order_book["ask_real_n_orders"]:
-            sell_implieds_only = True
-    if ask_price > order_book["ask_price"]:
-        if ask_impl_n_orders != 0 and \
-                ask_real_n_orders == 0:
-            sell_implieds_only = True
-    if ask_price < order_book["ask_price"]:
-        if order_book["ask_impl_n_orders"] != 0 and \
-                order_book["ask_real_n_orders"] == 0:
-            sell_implieds_only = True
-
-    buy_implieds_only = False
-    if bid_price == order_book["bid_price"]:
-        if bid_real_n_orders == order_book["bid_real_n_orders"]:
-            buy_implieds_only = True
-    if bid_price < order_book["bid_price"]:
-        if bid_impl_n_orders != 0 and \
-                bid_real_n_orders == 0:
-            buy_implieds_only = True
-    if bid_price < order_book["bid_price"]:
-        if order_book["bid_impl_n_orders"] != 0 and \
-                order_book["bid_real_n_orders"] == 0:
-            buy_implieds_only = True
-    order_book["implied_only"] = sell_implieds_only and buy_implieds_only
+    ask_unchanged = is_side_unchanged("ask", ask_price, ask_real_qty, ask_impl_qty,
+                                      ask_real_n_orders, ask_impl_n_orders, order_book)
+    ask_implied_only = is_side_update_purely_implied("ask", ask_price, ask_real_qty, ask_impl_qty,
+                                                     ask_real_n_orders, ask_impl_n_orders, order_book)
+    bid_unchanged = is_side_unchanged("bid", bid_price, bid_real_qty, bid_impl_qty,
+                                      bid_real_n_orders, bid_impl_n_orders, order_book)
+    bid_implied_only = is_side_update_purely_implied("bid", bid_price, bid_real_qty, bid_impl_qty,
+                                                     bid_real_n_orders, bid_impl_n_orders, order_book)
+
+    order_book["implied_only"] = (ask_implied_only and bid_unchanged)\
+                                 or (bid_implied_only and ask_unchanged) or (bid_implied_only and ask_implied_only)
 
     order_book["ask_price"] = ask_price
     order_book["ask_real_qty"] = ask_real_qty
     order_book["ask_impl_qty"] = ask_impl_qty
     order_book["ask_real_n_orders"] = ask_real_n_orders
     order_book["ask_impl_n_orders"] = ask_impl_n_orders
     order_book["bid_price"] = bid_price
```

### Comparing `recon_lw-2.0.0.dev5132270532/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5141842548/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/setup.py` & `recon_lw-2.0.0.dev5141842548/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5132270532/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5141842548/test/test_recon_ob.py`

 * *Files identical despite different names*

