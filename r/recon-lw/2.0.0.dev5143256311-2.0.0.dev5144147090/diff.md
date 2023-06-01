# Comparing `tmp/recon_lw-2.0.0.dev5143256311.tar.gz` & `tmp/recon_lw-2.0.0.dev5144147090.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5143256311.tar", last modified: Thu Jun  1 10:31:59 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5144147090.tar", last modified: Thu Jun  1 12:13:14 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5143256311.tar` & `recon_lw-2.0.0.dev5144147090.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 10:31:39.000000 recon_lw-2.0.0.dev5143256311/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33163 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob_cross_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 10:31:59.000000 recon_lw-2.0.0.dev5143256311/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 10:31:16.000000 recon_lw-2.0.0.dev5143256311/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-01 12:12:50.000000 recon_lw-2.0.0.dev5144147090/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13270 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33169 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22181 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob_cross_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 12:13:14.000000 recon_lw-2.0.0.dev5144147090/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-01 12:12:21.000000 recon_lw-2.0.0.dev5144147090/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,20 +634,20 @@
 
 def ob_top_clean_book(str_time_of_event, order_book: dict) -> tuple:
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
-    order_book["ask_price"] = 0
+    order_book["ask_price"] = None
     order_book["ask_real_qty"] = 0
     order_book["ask_impl_qty"] = 0
     order_book["ask_real_n_orders"] = 0
     order_book["ask_impl_n_orders"] = 0
-    order_book["bid_price"] = 0
+    order_book["bid_price"] = None
     order_book["bid_real_qty"] = 0
     order_book["bid_impl_qty"] = 0
     order_book["bid_real_n_orders"] = 0
     order_book["bid_impl_n_orders"] = 0
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 1
```

### Comparing `recon_lw-2.0.0.dev5143256311/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5144147090/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/setup.py` & `recon_lw-2.0.0.dev5144147090/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5143256311/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5144147090/test/test_recon_ob.py`

 * *Files identical despite different names*

