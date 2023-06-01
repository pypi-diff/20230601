# Comparing `tmp/island-1.1.1.tar.gz` & `tmp/island-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/island-1.1.1.tar", last modified: Wed Aug 28 21:21:00 2019, max compression
+gzip compressed data, was "dist/island-1.1.2.tar", last modified: Tue Sep 17 21:03:39 2019, max compression
```

## Comparing `island-1.1.1.tar` & `island-1.1.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-08-28 21:21:00.000000 island-1.1.1/
--rw-r--r--   0 heero     (1000) users      (985)       38 2019-08-28 21:18:08.000000 island-1.1.1/MANIFEST.in
--rw-r--r--   0 heero     (1000) users      (985)     4675 2019-08-28 21:21:00.000000 island-1.1.1/PKG-INFO
--rw-r--r--   0 heero     (1000) users      (985)     3129 2019-08-28 21:18:06.000000 island-1.1.1/README.md
-drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-08-28 21:21:00.000000 island-1.1.1/bin/
--rwxr-xr-x   0 heero     (1000) users      (985)      188 2019-05-08 13:41:44.000000 island-1.1.1/bin/island
-drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-08-28 21:21:00.000000 island-1.1.1/island/
--rwxr-xr-x   0 heero     (1000) users      (985)     8313 2019-08-28 21:18:06.000000 island-1.1.1/island/__init__.py
-drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-08-28 21:21:00.000000 island-1.1.1/island/actions/
--rw-r--r--   0 heero     (1000) users      (985)     2732 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_checkout.py
--rw-r--r--   0 heero     (1000) users      (985)     2539 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_command.py
--rw-r--r--   0 heero     (1000) users      (985)     3253 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_commit.py
--rw-r--r--   0 heero     (1000) users      (985)     2582 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_deliver-push.py
--rw-r--r--   0 heero     (1000) users      (985)     4780 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_deliver.py
--rw-r--r--   0 heero     (1000) users      (985)     3148 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_fetch.py
--rw-r--r--   0 heero     (1000) users      (985)     3108 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_init.py
--rw-r--r--   0 heero     (1000) users      (985)     2132 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_manifest-checkout.py
--rw-r--r--   0 heero     (1000) users      (985)     2000 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_manifest-deliver-push.py
--rw-r--r--   0 heero     (1000) users      (985)     6299 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_manifest-deliver.py
--rw-r--r--   0 heero     (1000) users      (985)     1895 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_manifest-status.py
--rw-r--r--   0 heero     (1000) users      (985)     1726 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_manifest-sync.py
--rw-r--r--   0 heero     (1000) users      (985)     3782 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_push.py
--rw-r--r--   0 heero     (1000) users      (985)     3027 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_status.py
--rw-r--r--   0 heero     (1000) users      (985)     6316 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_sync-local.py
--rw-r--r--   0 heero     (1000) users      (985)     6922 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_sync.py
--rw-r--r--   0 heero     (1000) users      (985)     2923 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_volatile-add.py
--rw-r--r--   0 heero     (1000) users      (985)     1638 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_volatile-list.py
--rw-r--r--   0 heero     (1000) users      (985)     3608 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/islandAction_volatile-remove.py
--rw-r--r--   0 heero     (1000) users      (985)    18420 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/status.py
--rw-r--r--   0 heero     (1000) users      (985)     1523 2019-08-28 21:18:06.000000 island-1.1.1/island/actions/update_links.py
--rw-r--r--   0 heero     (1000) users      (985)     4478 2019-08-28 21:18:06.000000 island-1.1.1/island/actions.py
--rw-r--r--   0 heero     (1000) users      (985)    13449 2019-08-28 21:18:06.000000 island-1.1.1/island/commands.py
--rw-r--r--   0 heero     (1000) users      (985)     4854 2019-08-28 21:18:06.000000 island-1.1.1/island/config.py
--rw-r--r--   0 heero     (1000) users      (985)     4264 2019-08-28 21:18:06.000000 island-1.1.1/island/env.py
--rw-r--r--   0 heero     (1000) users      (985)        0 2019-08-28 21:18:06.000000 island-1.1.1/island/git.py
--rw-r--r--   0 heero     (1000) users      (985)      527 2019-08-28 21:18:06.000000 island-1.1.1/island/host.py
--rw-r--r--   0 heero     (1000) users      (985)      326 2019-08-28 21:18:06.000000 island-1.1.1/island/link_config.py
--rw-r--r--   0 heero     (1000) users      (985)    19989 2019-08-28 21:18:06.000000 island-1.1.1/island/manifest.py
--rw-r--r--   0 heero     (1000) users      (985)     3134 2019-08-28 21:18:06.000000 island-1.1.1/island/multiprocess.py
--rw-r--r--   0 heero     (1000) users      (985)     1606 2019-08-28 21:18:06.000000 island-1.1.1/island/repo_config.py
--rw-r--r--   0 heero     (1000) users      (985)    10046 2019-08-28 21:18:06.000000 island-1.1.1/island/tools.py
-drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/
--rw-r--r--   0 heero     (1000) users      (985)     4675 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/PKG-INFO
--rw-r--r--   0 heero     (1000) users      (985)     1318 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/SOURCES.txt
--rw-r--r--   0 heero     (1000) users      (985)        1 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/dependency_links.txt
--rw-r--r--   0 heero     (1000) users      (985)        1 2019-05-08 13:41:44.000000 island-1.1.1/island.egg-info/not-zip-safe
--rw-r--r--   0 heero     (1000) users      (985)       18 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/requires.txt
--rw-r--r--   0 heero     (1000) users      (985)       22 2019-08-28 21:21:00.000000 island-1.1.1/island.egg-info/top_level.txt
--rw-r--r--   0 heero     (1000) users      (985)       38 2019-08-28 21:21:00.000000 island-1.1.1/setup.cfg
--rwxr-xr-x   0 heero     (1000) users      (985)     1851 2019-08-28 21:18:49.000000 island-1.1.1/setup.py
--rw-r--r--   0 heero     (1000) users      (985)        5 2019-08-28 21:18:49.000000 island-1.1.1/version.txt
+drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-09-17 21:03:39.000000 island-1.1.2/
+-rw-r--r--   0 heero     (1000) users      (985)       38 2019-08-28 21:18:08.000000 island-1.1.2/MANIFEST.in
+-rw-r--r--   0 heero     (1000) users      (985)     4675 2019-09-17 21:03:39.000000 island-1.1.2/PKG-INFO
+-rw-r--r--   0 heero     (1000) users      (985)     3129 2019-08-28 21:18:06.000000 island-1.1.2/README.md
+drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-09-17 21:03:39.000000 island-1.1.2/bin/
+-rwxr-xr-x   0 heero     (1000) users      (985)      188 2019-05-08 13:41:44.000000 island-1.1.2/bin/island
+drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-09-17 21:03:39.000000 island-1.1.2/island/
+-rwxr-xr-x   0 heero     (1000) users      (985)     8313 2019-08-28 21:18:06.000000 island-1.1.2/island/__init__.py
+drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-09-17 21:03:39.000000 island-1.1.2/island/actions/
+-rw-r--r--   0 heero     (1000) users      (985)     2732 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_checkout.py
+-rw-r--r--   0 heero     (1000) users      (985)     2539 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_command.py
+-rw-r--r--   0 heero     (1000) users      (985)     3253 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_commit.py
+-rw-r--r--   0 heero     (1000) users      (985)     2582 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_deliver-push.py
+-rw-r--r--   0 heero     (1000) users      (985)     4780 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_deliver.py
+-rw-r--r--   0 heero     (1000) users      (985)     3148 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_fetch.py
+-rw-r--r--   0 heero     (1000) users      (985)     3108 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_init.py
+-rw-r--r--   0 heero     (1000) users      (985)     2132 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_manifest-checkout.py
+-rw-r--r--   0 heero     (1000) users      (985)     2000 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_manifest-deliver-push.py
+-rw-r--r--   0 heero     (1000) users      (985)     6299 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_manifest-deliver.py
+-rw-r--r--   0 heero     (1000) users      (985)     1895 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_manifest-status.py
+-rw-r--r--   0 heero     (1000) users      (985)     1726 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_manifest-sync.py
+-rw-r--r--   0 heero     (1000) users      (985)     3782 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_push.py
+-rw-r--r--   0 heero     (1000) users      (985)     3040 2019-09-17 21:03:11.000000 island-1.1.2/island/actions/islandAction_status.py
+-rw-r--r--   0 heero     (1000) users      (985)     6316 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_sync-local.py
+-rw-r--r--   0 heero     (1000) users      (985)     6922 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_sync.py
+-rw-r--r--   0 heero     (1000) users      (985)     2923 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_volatile-add.py
+-rw-r--r--   0 heero     (1000) users      (985)     1638 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_volatile-list.py
+-rw-r--r--   0 heero     (1000) users      (985)     3608 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/islandAction_volatile-remove.py
+-rw-r--r--   0 heero     (1000) users      (985)    18420 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/status.py
+-rw-r--r--   0 heero     (1000) users      (985)     1523 2019-08-28 21:18:06.000000 island-1.1.2/island/actions/update_links.py
+-rw-r--r--   0 heero     (1000) users      (985)     4478 2019-08-28 21:18:06.000000 island-1.1.2/island/actions.py
+-rw-r--r--   0 heero     (1000) users      (985)    13449 2019-08-28 21:18:06.000000 island-1.1.2/island/commands.py
+-rw-r--r--   0 heero     (1000) users      (985)     4854 2019-08-28 21:18:06.000000 island-1.1.2/island/config.py
+-rw-r--r--   0 heero     (1000) users      (985)     4264 2019-08-28 21:18:06.000000 island-1.1.2/island/env.py
+-rw-r--r--   0 heero     (1000) users      (985)        0 2019-08-28 21:18:06.000000 island-1.1.2/island/git.py
+-rw-r--r--   0 heero     (1000) users      (985)      527 2019-08-28 21:18:06.000000 island-1.1.2/island/host.py
+-rw-r--r--   0 heero     (1000) users      (985)      326 2019-08-28 21:18:06.000000 island-1.1.2/island/link_config.py
+-rw-r--r--   0 heero     (1000) users      (985)    19989 2019-08-28 21:18:06.000000 island-1.1.2/island/manifest.py
+-rw-r--r--   0 heero     (1000) users      (985)     3134 2019-08-28 21:18:06.000000 island-1.1.2/island/multiprocess.py
+-rw-r--r--   0 heero     (1000) users      (985)     1606 2019-08-28 21:18:06.000000 island-1.1.2/island/repo_config.py
+-rw-r--r--   0 heero     (1000) users      (985)    10046 2019-08-28 21:18:06.000000 island-1.1.2/island/tools.py
+drwxr-xr-x   0 heero     (1000) users      (985)        0 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/
+-rw-r--r--   0 heero     (1000) users      (985)     4675 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/PKG-INFO
+-rw-r--r--   0 heero     (1000) users      (985)     1318 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/SOURCES.txt
+-rw-r--r--   0 heero     (1000) users      (985)        1 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/dependency_links.txt
+-rw-r--r--   0 heero     (1000) users      (985)        1 2019-05-08 13:41:44.000000 island-1.1.2/island.egg-info/not-zip-safe
+-rw-r--r--   0 heero     (1000) users      (985)       18 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/requires.txt
+-rw-r--r--   0 heero     (1000) users      (985)       22 2019-09-17 21:03:39.000000 island-1.1.2/island.egg-info/top_level.txt
+-rw-r--r--   0 heero     (1000) users      (985)       38 2019-09-17 21:03:39.000000 island-1.1.2/setup.cfg
+-rwxr-xr-x   0 heero     (1000) users      (985)     1851 2019-08-28 21:18:49.000000 island-1.1.2/setup.py
+-rw-r--r--   0 heero     (1000) users      (985)        5 2019-09-17 21:03:11.000000 island-1.1.2/version.txt
```

### Comparing `island-1.1.1/PKG-INFO` & `island-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: island
-Version: 1.1.1
+Version: 1.1.2
 Summary: island generic source manager (like repo in simple mode)
 Home-page: http://github.com/HeeroYui/island
 Author: Edouard DUPIN
 Author-email: yui.heero@gmail.com
 License: MPL-2
 Description: Island
         =======
```

### Comparing `island-1.1.1/README.md` & `island-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/__init__.py` & `island-1.1.2/island/__init__.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_checkout.py` & `island-1.1.2/island/actions/islandAction_checkout.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_command.py` & `island-1.1.2/island/actions/islandAction_command.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_commit.py` & `island-1.1.2/island/actions/islandAction_commit.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_deliver-push.py` & `island-1.1.2/island/actions/islandAction_deliver-push.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_deliver.py` & `island-1.1.2/island/actions/islandAction_deliver.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_fetch.py` & `island-1.1.2/island/actions/islandAction_fetch.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_init.py` & `island-1.1.2/island/actions/islandAction_init.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_manifest-checkout.py` & `island-1.1.2/island/actions/islandAction_manifest-checkout.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_manifest-deliver-push.py` & `island-1.1.2/island/actions/islandAction_manifest-deliver-push.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_manifest-deliver.py` & `island-1.1.2/island/actions/islandAction_manifest-deliver.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_manifest-status.py` & `island-1.1.2/island/actions/islandAction_manifest-status.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_manifest-sync.py` & `island-1.1.2/island/actions/islandAction_manifest-sync.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_push.py` & `island-1.1.2/island/actions/islandAction_push.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_status.py` & `island-1.1.2/island/actions/islandAction_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,14 @@
 	status.display_status(elem, argument_remote_name, argument_display_tag, id_element, base_display)
 	
 	is_behind = False
 	for elem in all_project:
 		id_element += 1
 		base_display = tools.get_list_base_display(id_element, len(all_project), elem)
 		ret = status.display_status(elem, argument_remote_name, argument_display_tag, id_element, base_display)
-		if ret != None:
+		if ret != None and ret != 0:
 			is_behind = True
 	
 	if is_behind == True:
 		return env.ret_action_need_updtate
```

### Comparing `island-1.1.1/island/actions/islandAction_sync-local.py` & `island-1.1.2/island/actions/islandAction_sync-local.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_sync.py` & `island-1.1.2/island/actions/islandAction_sync.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_volatile-add.py` & `island-1.1.2/island/actions/islandAction_volatile-add.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_volatile-list.py` & `island-1.1.2/island/actions/islandAction_volatile-list.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/islandAction_volatile-remove.py` & `island-1.1.2/island/actions/islandAction_volatile-remove.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/status.py` & `island-1.1.2/island/actions/status.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions/update_links.py` & `island-1.1.2/island/actions/update_links.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/actions.py` & `island-1.1.2/island/actions.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/commands.py` & `island-1.1.2/island/commands.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/config.py` & `island-1.1.2/island/config.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/env.py` & `island-1.1.2/island/env.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/host.py` & `island-1.1.2/island/host.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/manifest.py` & `island-1.1.2/island/manifest.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/multiprocess.py` & `island-1.1.2/island/multiprocess.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/repo_config.py` & `island-1.1.2/island/repo_config.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island/tools.py` & `island-1.1.2/island/tools.py`

 * *Files identical despite different names*

### Comparing `island-1.1.1/island.egg-info/PKG-INFO` & `island-1.1.2/island.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: island
-Version: 1.1.1
+Version: 1.1.2
 Summary: island generic source manager (like repo in simple mode)
 Home-page: http://github.com/HeeroYui/island
 Author: Edouard DUPIN
 Author-email: yui.heero@gmail.com
 License: MPL-2
 Description: Island
         =======
```

### Comparing `island-1.1.1/island.egg-info/SOURCES.txt` & `island-1.1.2/island.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `island-1.1.1/setup.py` & `island-1.1.2/setup.py`

 * *Files identical despite different names*

