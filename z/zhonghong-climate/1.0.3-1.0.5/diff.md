# Comparing `tmp/zhonghong_climate-1.0.3.tar.gz` & `tmp/zhonghong_climate-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhonghong_climate-1.0.3.tar", last modified: Wed May 31 06:19:51 2023, max compression
+gzip compressed data, was "zhonghong_climate-1.0.5.tar", last modified: Thu Jun  1 01:09:43 2023, max compression
```

## Comparing `zhonghong_climate-1.0.3.tar` & `zhonghong_climate-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/
--rw-rw-rw-   0        0        0      752 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.861629 zhonghong_climate-1.0.3/zhonghong_climate/
--rw-rw-rw-   0        0        0       31 2023-05-30 07:22:47.000000 zhonghong_climate-1.0.3/zhonghong_climate/__init__.py
--rw-rw-rw-   0        0        0     3485 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/zhonghong_climate/helper.py
--rw-rw-rw-   0        0        0     8990 2023-05-31 06:15:04.000000 zhonghong_climate-1.0.3/zhonghong_climate/hub.py
--rw-rw-rw-   0        0        0     4958 2023-05-31 06:15:14.000000 zhonghong_climate-1.0.3/zhonghong_climate/hvac.py
--rw-rw-rw-   0        0        0     8297 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/zhonghong_climate/protocol.py
--rw-rw-rw-   0        0        0       23 2023-05-31 06:15:17.000000 zhonghong_climate-1.0.3/zhonghong_climate/version.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.882572 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/
--rw-rw-rw-   0        0        0      752 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:43.876733 zhonghong_climate-1.0.5/
+-rw-rw-rw-   0        0        0      752 2023-06-01 01:09:43.872604 zhonghong_climate-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:09:43.876733 zhonghong_climate-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:43.862630 zhonghong_climate-1.0.5/zhonghong_climate/
+-rw-rw-rw-   0        0        0       31 2023-05-30 07:22:47.000000 zhonghong_climate-1.0.5/zhonghong_climate/__init__.py
+-rw-rw-rw-   0        0        0     3485 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.5/zhonghong_climate/helper.py
+-rw-rw-rw-   0        0        0     9349 2023-06-01 01:05:29.000000 zhonghong_climate-1.0.5/zhonghong_climate/hub.py
+-rw-rw-rw-   0        0        0     4958 2023-05-31 06:15:14.000000 zhonghong_climate-1.0.5/zhonghong_climate/hvac.py
+-rw-rw-rw-   0        0        0     8297 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.5/zhonghong_climate/protocol.py
+-rw-rw-rw-   0        0        0       23 2023-06-01 01:05:41.000000 zhonghong_climate-1.0.5/zhonghong_climate/version.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:09:43.871601 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/
+-rw-rw-rw-   0        0        0      752 2023-06-01 01:09:43.000000 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-06-01 01:09:43.000000 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:09:43.000000 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 01:09:43.000000 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 01:09:43.000000 zhonghong_climate-1.0.5/zhonghong_climate.egg-info/top_level.txt
```

### Comparing `zhonghong_climate-1.0.3/PKG-INFO` & `zhonghong_climate-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhonghong_climate
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zhonghong_climate-1.0.3/setup.py` & `zhonghong_climate-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.3/zhonghong_climate/helper.py` & `zhonghong_climate-1.0.5/zhonghong_climate/helper.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.3/zhonghong_climate/hub.py` & `zhonghong_climate-1.0.5/zhonghong_climate/hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -200,14 +200,20 @@
         if self.sock:
             logger.info('Closing socket.')
             self.sock.close()
             self.sock = None
 
         for thread in self._threads:
             thread.join()
+            
+    def device_in_list(self, addr_out, addr_in, device_list) -> bool:
+        for (item_addr_out, item_addr_in) in device_list:
+            if addr_out == item_addr_out and item_addr_in == addr_in:
+                return True
+        return False
 
     def discovery_ac(self):
         assert not self._listening
 
         if self.sock is None:
             self.open_socket()
 
@@ -230,19 +236,18 @@
                 logger.error("No response from gateway")
 
             for ac_data in helper.get_ac_data(data):
                 if ac_data.header != request_data.header:
                     logger.debug("header not match: %s != %s",
                                  request_data.header, ac_data.header)
                     continue
-
                 for ac_online in ac_data:
                     assert isinstance(ac_online, protocol.AcOnline)
-                    ret.append((ac_online.addr_out, ac_online.addr_in))
-
+                    if not self.device_in_list(ac_online.addr_out, ac_online.addr_in, ret):
+                        ret.append((ac_online.addr_out, ac_online.addr_in))
                 discovered = True
 
         return ret
 
     def query_all_status(self) -> None:
         request_data = protocol.AcData()
         request_data.header = protocol.Header(
```

### Comparing `zhonghong_climate-1.0.3/zhonghong_climate/hvac.py` & `zhonghong_climate-1.0.5/zhonghong_climate/hvac.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.3/zhonghong_climate/protocol.py` & `zhonghong_climate-1.0.5/zhonghong_climate/protocol.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.3/zhonghong_climate.egg-info/PKG-INFO` & `zhonghong_climate-1.0.5/zhonghong_climate.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhonghong-climate
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
 Classifier: Development Status :: 4 - Beta
```

