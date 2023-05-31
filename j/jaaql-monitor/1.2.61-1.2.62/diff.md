# Comparing `tmp/jaaql-monitor-1.2.61.tar.gz` & `tmp/jaaql-monitor-1.2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.61.tar", last modified: Wed May 31 20:49:33 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.62.tar", last modified: Wed May 31 22:03:23 2023, max compression
```

## Comparing `jaaql-monitor-1.2.61.tar` & `jaaql-monitor-1.2.62.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.461475 jaaql-monitor-1.2.61/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.61/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-05-31 20:49:33.461475 jaaql-monitor-1.2.61/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.61/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.458476 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 20:49:33.000000 jaaql-monitor-1.2.61/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 20:49:33.460475 jaaql-monitor-1.2.61/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.61/monitor/__init__.py
--rw-rw-rw-   0        0        0    27616 2023-05-31 20:48:58.000000 jaaql-monitor-1.2.61/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-05-31 20:49:18.000000 jaaql-monitor-1.2.61/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-05-31 20:49:33.462475 jaaql-monitor-1.2.61/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.61/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:03:23.185583 jaaql-monitor-1.2.62/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.62/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-05-31 22:03:23.185583 jaaql-monitor-1.2.62/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.62/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:03:23.181595 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-05-31 22:03:23.000000 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-31 22:03:23.000000 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:03:23.000000 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 22:03:23.000000 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 22:03:23.000000 jaaql-monitor-1.2.62/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 22:03:23.184583 jaaql-monitor-1.2.62/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.62/monitor/__init__.py
+-rw-rw-rw-   0        0        0    28188 2023-05-31 22:02:59.000000 jaaql-monitor-1.2.62/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-05-31 22:03:12.000000 jaaql-monitor-1.2.62/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:03:23.185583 jaaql-monitor-1.2.62/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.62/setup.py
```

### Comparing `jaaql-monitor-1.2.61/LICENSE.txt` & `jaaql-monitor-1.2.62/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.61/PKG-INFO` & `jaaql-monitor-1.2.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.61
+Version: 1.2.62
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.61/README.md` & `jaaql-monitor-1.2.62/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.61/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.62/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.61
+Version: 1.2.62
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.61/monitor/main.py` & `jaaql-monitor-1.2.62/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,20 @@
 
 LINE_LENGTH_MAX = 115
 ROWS_MAX = 25
 
 METHOD__post = "POST"
 METHOD__get = "GET"
 
-ARGS__encoded_config = ['-e', '--encoded-config']
+ARGS__encoded_config = ['--encoded-config']
 ARGS__config = ['-c', '--config']
 ARGS__folder_config = ['-f', '--folder-config']
 ARGS__parameter = ['-p', '--parameter']
+ARGS__single_query = ['-s', '--single-query']
+ARGS__environment = ['-e', '--environment-file']
 
 
 class JAAQLMonitorException(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
@@ -555,15 +557,15 @@
     else:
         state.file_name = file_name
 
     state.override_url = override_url
 
     state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
-    state.single_query = len([arg for arg in args if arg in ['-s', '--single-query']]) != 0
+    state.single_query = len([arg for arg in args if arg in ARGS__single_query]) != 0
 
     if state.is_verbose:
         print_version()
 
     for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__parameter:
             continue
@@ -579,14 +581,26 @@
 
         if parameter_name in state.parameters:
             print_error(state, "The parameter '" + parameter_name + "' has already been supplied")
 
         state.parameters[parameter_name] = parameter_value
 
     for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__environment:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The environment flag is the last argument. You need to supply a file")
+
+        parameter_file = args[arg_idx + 1]
+
+        for line in open(parameter_file, "r").readlines():
+            state.parameters[line.split("=")[0]] = "=".join(line.split("=")[1:])
+
+    for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__folder_config:
             continue
 
         if arg_idx == len(args) - 1:
             print_error(state, "The folder config flag is the last argument. You need to supply a file")
 
         configuration_folder = args[arg_idx + 1]
@@ -638,23 +652,23 @@
                                                                        b64d(content_split[2]).decode(), db, state.override_url)
 
     deal_with_input(state, file_content)
 
 
 def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]],
                override_url: str):
-    args = ["-s"]
+    args = [ARGS__single_query[0]]
 
     for config in configs:
-        args.append("-c")
+        args.append(ARGS__config[0])
         args.append(config[0])
         args.append(config[1])
 
     for encoded_config in encoded_configs:
-        args.append("-e")
+        args.append(ARGS__encoded_config[0])
         args.append(encoded_config[0])
         db_part = ""
         if encoded_config[4]:
             db_part = ":" + b64e(encoded_config[4].encode()).decode()
         args.append(b64e(encoded_config[1].encode()).decode() + ":" + b64e(encoded_config[2].encode()).decode() + ":" +
                     b64e(encoded_config[3].encode()).decode() + db_part)
```

### Comparing `jaaql-monitor-1.2.61/setup.py` & `jaaql-monitor-1.2.62/setup.py`

 * *Files identical despite different names*

