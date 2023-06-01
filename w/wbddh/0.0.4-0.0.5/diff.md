# Comparing `tmp/wbddh-0.0.4-py3-none-any.whl.zip` & `tmp/wbddh-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8866 bytes, number of entries: 11
+Zip file size: 9120 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-15 19:53 wbddh/__init__.py
 -rw-rw-rw-  2.0 fat      990 b- defN 23-May-15 19:53 wbddh/exceptions.py
--rw-rw-rw-  2.0 fat     2419 b- defN 23-May-19 15:09 wbddh/request_manager.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-Jun-01 13:39 wbddh/request_manager.py
 -rw-rw-rw-  2.0 fat     8796 b- defN 23-May-11 22:36 wbddh/session.py
 -rw-rw-rw-  2.0 fat     6218 b- defN 23-May-21 04:48 wbddh/session_manager.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-May-13 18:53 wbddh/test.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-May-11 22:36 wbddh/utils.py
--rw-rw-rw-  2.0 fat      543 b- defN 23-May-21 04:49 wbddh-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-21 04:49 wbddh-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-21 04:49 wbddh-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      810 b- defN 23-May-21 04:49 wbddh-0.0.4.dist-info/RECORD
-11 files, 21638 bytes uncompressed, 7514 bytes compressed:  65.3%
+-rw-rw-rw-  2.0 fat      543 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-01 13:39 wbddh-0.0.5.dist-info/RECORD
+11 files, 22629 bytes uncompressed, 7768 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: wbddh/test.py
 Comment: 
 
 Filename: wbddh/utils.py
 Comment: 
 
-Filename: wbddh-0.0.4.dist-info/METADATA
+Filename: wbddh-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: wbddh-0.0.4.dist-info/WHEEL
+Filename: wbddh-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: wbddh-0.0.4.dist-info/top_level.txt
+Filename: wbddh-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: wbddh-0.0.4.dist-info/RECORD
+Filename: wbddh-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbddh/request_manager.py

```diff
@@ -16,15 +16,37 @@
     '''
     if session:
         session.check_tokens()
         return requests.get(get_endpoint(endpoint, session), params=params, verify=session.verify, headers=session.get_headers(headers))
     else:
         return requests.get(get_endpoint(endpoint), params=params)
 
+def try_get(endpoint, params=None, headers=None, session=None, num_try=3, interval=300):
+    '''Repeat sending a GET request until it succeeds or it tries {num_try} times
 
+    Additional arguments:
+        num_try:        number of tries
+        interval:       interval between tries in seconds
+    '''
+    count = 0
+    while True:
+        try:
+            if session:
+                session.check_tokens()
+                response = requests.get(get_endpoint(endpoint, session), params=params, verify=session.verify, headers=session.get_headers(headers))
+            else:
+                response = requests.get(get_endpoint(endpoint), params=params)
+            count = count + 1
+        except requests.exceptions.RequestException as e:
+            print (f"[{count} try] An error occured: ", e)
+
+        if response.status_code == 200:
+            return response
+        elif count > num_try:
+            raise Exception(f"Request failed after {count} tries.")
 
 def post(endpoint, params=None, json=None, headers=None, session=None):
     '''Send a POST request
 
     Arguments:
         endpoint:		the endpoint (e.g., "dataset/listpage")
         json:			data object
```

## Comparing `wbddh-0.0.4.dist-info/METADATA` & `wbddh-0.0.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbddh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python wrapper for DDH Open API
 Home-page: https://github.com/WB-DECIS/WBDDH
 Author: DECIS
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Provides-Extra: admin
 Requires-Dist: msal ; extra == 'admin'
```

