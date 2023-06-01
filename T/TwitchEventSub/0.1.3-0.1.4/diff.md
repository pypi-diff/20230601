# Comparing `tmp/TwitchEventSub-0.1.3.tar.gz` & `tmp/TwitchEventSub-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TwitchEventSub-0.1.3.tar", last modified: Wed Jan  4 05:34:51 2023, max compression
+gzip compressed data, was "TwitchEventSub-0.1.4.tar", last modified: Thu Jun  1 14:44:49 2023, max compression
```

## Comparing `TwitchEventSub-0.1.3.tar` & `TwitchEventSub-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 05:34:51.961593 TwitchEventSub-0.1.3/
--rw-rw-rw-   0        0        0     1089 2022-12-28 18:10:43.000000 TwitchEventSub-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      695 2023-01-04 05:34:51.961593 TwitchEventSub-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      102 2022-12-28 18:10:43.000000 TwitchEventSub-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-04 05:34:51.828876 TwitchEventSub-0.1.3/TwitchEventSub/
--rw-rw-rw-   0        0        0      122 2022-12-27 23:11:38.000000 TwitchEventSub-0.1.3/TwitchEventSub/__init__.py
--rw-rw-rw-   0        0        0     3037 2022-12-30 01:58:15.000000 TwitchEventSub-0.1.3/TwitchEventSub/authentication.py
-drwxrwxrwx   0        0        0        0 2023-01-04 05:34:51.958667 TwitchEventSub-0.1.3/TwitchEventSub/event_types/
--rw-rw-rw-   0        0        0        0 2022-12-27 22:58:44.000000 TwitchEventSub-0.1.3/TwitchEventSub/event_types/__init__.py
--rw-rw-rw-   0        0        0     3139 2022-12-28 08:33:37.000000 TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_scopes.py
--rw-rw-rw-   0        0        0     2607 2022-12-27 23:12:53.000000 TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_types.py
--rw-rw-rw-   0        0        0     2462 2022-12-27 23:12:53.000000 TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_versions.py
--rw-rw-rw-   0        0        0      127 2022-12-28 17:23:30.000000 TwitchEventSub-0.1.3/TwitchEventSub/exceptions.py
--rw-rw-rw-   0        0        0    19701 2023-01-04 05:32:42.000000 TwitchEventSub-0.1.3/TwitchEventSub/twitch_event_sub.py
-drwxrwxrwx   0        0        0        0 2023-01-04 05:34:51.845472 TwitchEventSub-0.1.3/TwitchEventSub.egg-info/
--rw-rw-rw-   0        0        0      695 2023-01-04 05:34:51.000000 TwitchEventSub-0.1.3/TwitchEventSub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-01-04 05:34:51.000000 TwitchEventSub-0.1.3/TwitchEventSub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 05:34:51.000000 TwitchEventSub-0.1.3/TwitchEventSub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-01-04 05:34:51.000000 TwitchEventSub-0.1.3/TwitchEventSub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-04 05:34:51.963550 TwitchEventSub-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-01-04 05:24:51.000000 TwitchEventSub-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:44:49.533462 TwitchEventSub-0.1.4/
+-rw-rw-rw-   0        0        0     1089 2022-12-28 18:10:43.000000 TwitchEventSub-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-06-01 14:44:49.533462 TwitchEventSub-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2022-12-28 18:10:43.000000 TwitchEventSub-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:44:49.470416 TwitchEventSub-0.1.4/TwitchEventSub/
+-rw-rw-rw-   0        0        0      122 2022-12-27 23:11:38.000000 TwitchEventSub-0.1.4/TwitchEventSub/__init__.py
+-rw-rw-rw-   0        0        0     3037 2022-12-30 01:58:15.000000 TwitchEventSub-0.1.4/TwitchEventSub/authentication.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:44:49.528440 TwitchEventSub-0.1.4/TwitchEventSub/event_types/
+-rw-rw-rw-   0        0        0        0 2022-12-27 22:58:44.000000 TwitchEventSub-0.1.4/TwitchEventSub/event_types/__init__.py
+-rw-rw-rw-   0        0        0     3139 2022-12-28 08:33:37.000000 TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_scopes.py
+-rw-rw-rw-   0        0        0     2607 2022-12-27 23:12:53.000000 TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_types.py
+-rw-rw-rw-   0        0        0     2462 2022-12-27 23:12:53.000000 TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_versions.py
+-rw-rw-rw-   0        0        0      127 2022-12-28 17:23:30.000000 TwitchEventSub-0.1.4/TwitchEventSub/exceptions.py
+-rw-rw-rw-   0        0        0    19696 2023-06-01 14:40:11.000000 TwitchEventSub-0.1.4/TwitchEventSub/twitch_event_sub.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:44:49.487372 TwitchEventSub-0.1.4/TwitchEventSub.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-06-01 14:44:49.000000 TwitchEventSub-0.1.4/TwitchEventSub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-06-01 14:44:49.000000 TwitchEventSub-0.1.4/TwitchEventSub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:44:49.000000 TwitchEventSub-0.1.4/TwitchEventSub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 14:44:49.000000 TwitchEventSub-0.1.4/TwitchEventSub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-01 14:44:49.542402 TwitchEventSub-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2023-06-01 14:39:58.000000 TwitchEventSub-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:44:49.531432 TwitchEventSub-0.1.4/tests/
+-rw-rw-rw-   0        0        0      715 2022-12-30 01:59:17.000000 TwitchEventSub-0.1.4/tests/test_handler.py
```

### Comparing `TwitchEventSub-0.1.3/LICENSE` & `TwitchEventSub-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `TwitchEventSub-0.1.3/PKG-INFO` & `TwitchEventSub-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TwitchEventSub
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python package for receiving EventSub notifications from Twitch over WebSocket
 Home-page: https://github.com/CPSuperstore/TwitchEventSub
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/TwitchEventSub/issues
 Keywords: Twitch,EventSub,Bot,WebSocket,Channel Points,livestream
```

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub/authentication.py` & `TwitchEventSub-0.1.4/TwitchEventSub/authentication.py`

 * *Files identical despite different names*

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_scopes.py` & `TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_scopes.py`

 * *Files identical despite different names*

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_types.py` & `TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_types.py`

 * *Files identical despite different names*

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub/event_types/event_versions.py` & `TwitchEventSub-0.1.4/TwitchEventSub/event_types/event_versions.py`

 * *Files identical despite different names*

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub/twitch_event_sub.py` & `TwitchEventSub-0.1.4/TwitchEventSub/twitch_event_sub.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class TwitchEventSub(abc.ABC):
     def __init__(
             self, client_id: str, client_secret: str, subscribed_events: typing.List[event_types.EventType],
             additional_scopes: typing.List[str] = None,
             persist_credentials: bool = True, credentials_path: str = "salts.json",
-            ws_url: str = 'wss://eventsub-beta.wss.twitch.tv/ws'
+            ws_url: str = 'wss://eventsub.wss.twitch.tv/ws'
     ):
         if additional_scopes is None:
             additional_scopes = []
 
         self._client_id = client_id
         self._client_secret = client_secret
         self._persist_credentials = persist_credentials
```

### Comparing `TwitchEventSub-0.1.3/TwitchEventSub.egg-info/PKG-INFO` & `TwitchEventSub-0.1.4/TwitchEventSub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TwitchEventSub
-Version: 0.1.3
+Version: 0.1.4
 Summary: The Python package for receiving EventSub notifications from Twitch over WebSocket
 Home-page: https://github.com/CPSuperstore/TwitchEventSub
 Author: CPSuperstore
 Author-email: cpsuperstoreinc@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CPSuperstore/TwitchEventSub/issues
 Keywords: Twitch,EventSub,Bot,WebSocket,Channel Points,livestream
```

### Comparing `TwitchEventSub-0.1.3/setup.py` & `TwitchEventSub-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = find_packages(where=".")
 
 if "tests" in packages:
     packages.remove("tests")
 
 setup(
     name='TwitchEventSub',
-    version='0.1.3',
+    version='0.1.4',
     packages=packages,
     url='https://github.com/CPSuperstore/TwitchEventSub',
     license='MIT',
     author='CPSuperstore',
     author_email='cpsuperstoreinc@gmail.com',
     description='The Python package for receiving EventSub notifications from Twitch over WebSocket',
     long_description=long_description,
```

