# Comparing `tmp/eva-shell-0.0.92.tar.gz` & `tmp/eva-shell-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eva-shell-0.0.92.tar", last modified: Thu May 11 15:47:04 2023, max compression
+gzip compressed data, was "eva-shell-0.0.93.tar", last modified: Wed May 31 23:34:47 2023, max compression
```

## Comparing `eva-shell-0.0.92.tar` & `eva-shell-0.0.93.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/
--rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.0.92/LICENSE
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-11 15:47:04.744640 eva-shell-0.0.92/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.0.92/README.md
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/bin/
--rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.0.92/bin/eva
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/eva4_shell/
--rw-r--r--   0 divisor   (1000) root         (0)       75 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/__init__.py
--rw-r--r--   0 divisor   (1000) root         (0)    47371 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/ap.py
--rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/charts.py
--rw-r--r--   0 divisor   (1000) root         (0)    51586 2023-05-04 21:53:31.000000 eva-shell-0.0.92/eva4_shell/cli.py
--rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/client.py
--rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/compl.py
--rw-r--r--   0 divisor   (1000) root         (0)      653 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/sharedobj.py
--rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/shell.py
--rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-05-02 01:18:10.000000 eva-shell-0.0.92/eva4_shell/tools.py
-drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-11 15:47:04.744640 eva-shell-0.0.92/eva_shell.egg-info/
--rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/PKG-INFO
--rw-r--r--   0 divisor   (1000) root         (0)      382 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/SOURCES.txt
--rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/dependency_links.txt
--rw-r--r--   0 divisor   (1000) root         (0)      166 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/requires.txt
--rw-r--r--   0 divisor   (1000) root         (0)       11 2023-05-11 15:47:04.000000 eva-shell-0.0.92/eva_shell.egg-info/top_level.txt
--rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-11 15:47:04.744640 eva-shell-0.0.92/setup.cfg
--rw-r--r--   0 divisor   (1000) root         (0)     1188 2023-05-04 21:53:31.000000 eva-shell-0.0.92/setup.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.545655 eva-shell-0.0.93/
+-rw-r--r--   0 divisor   (1000) root         (0)    10639 2022-06-30 23:31:07.000000 eva-shell-0.0.93/LICENSE
+-rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-31 23:34:47.545655 eva-shell-0.0.93/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)       19 2022-03-19 02:57:04.000000 eva-shell-0.0.93/README.md
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/bin/
+-rwxr-xr-x   0 divisor   (1000) root         (0)       73 2022-03-19 02:57:04.000000 eva-shell-0.0.93/bin/eva
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/eva4_shell/
+-rw-r--r--   0 divisor   (1000) root         (0)       75 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/__init__.py
+-rw-r--r--   0 divisor   (1000) root         (0)    47371 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/ap.py
+-rw-r--r--   0 divisor   (1000) root         (0)     7078 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/charts.py
+-rw-r--r--   0 divisor   (1000) root         (0)    51601 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/cli.py
+-rw-r--r--   0 divisor   (1000) root         (0)     2634 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/client.py
+-rw-r--r--   0 divisor   (1000) root         (0)     4332 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/compl.py
+-rw-r--r--   0 divisor   (1000) root         (0)      653 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/sharedobj.py
+-rw-r--r--   0 divisor   (1000) root         (0)     1701 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/shell.py
+-rw-r--r--   0 divisor   (1000) root         (0)    13863 2023-05-31 23:34:44.000000 eva-shell-0.0.93/eva4_shell/tools.py
+drwxr-xr-x   0 divisor   (1000) root         (0)        0 2023-05-31 23:34:47.541655 eva-shell-0.0.93/eva_shell.egg-info/
+-rw-r--r--   0 divisor   (1000) root         (0)      459 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/PKG-INFO
+-rw-r--r--   0 divisor   (1000) root         (0)      382 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 divisor   (1000) root         (0)        1 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 divisor   (1000) root         (0)      166 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/requires.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       11 2023-05-31 23:34:47.000000 eva-shell-0.0.93/eva_shell.egg-info/top_level.txt
+-rw-r--r--   0 divisor   (1000) root         (0)       38 2023-05-31 23:34:47.545655 eva-shell-0.0.93/setup.cfg
+-rw-r--r--   0 divisor   (1000) root         (0)     1188 2023-05-31 23:34:44.000000 eva-shell-0.0.93/setup.py
```

### Comparing `eva-shell-0.0.92/LICENSE` & `eva-shell-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/ap.py` & `eva-shell-0.0.93/eva4_shell/ap.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/charts.py` & `eva-shell-0.0.93/eva4_shell/charts.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/cli.py` & `eva-shell-0.0.93/eva4_shell/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,15 +646,15 @@
 
     def action_exec(self, i, status, value, priority, wait):
         params = dict(i=i, wait=wait)
         if priority is not None:
             params['priority'] = int(priority)
         action_params = {'status': int(status)}
         if value is not None:
-            action_params['value'] = format_value(value)
+            action_params['value'] = format_value(value, advanced=True)
         params['params'] = action_params
         result = call_rpc('action', params)
         if current_command.json:
             import uuid
             result['uuid'] = str(uuid.UUID(bytes=result['uuid']))
             print_result(result)
         else:
```

### Comparing `eva-shell-0.0.92/eva4_shell/client.py` & `eva-shell-0.0.93/eva4_shell/client.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/compl.py` & `eva-shell-0.0.93/eva4_shell/compl.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/sharedobj.py` & `eva-shell-0.0.93/eva4_shell/sharedobj.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/shell.py` & `eva-shell-0.0.93/eva4_shell/shell.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/eva4_shell/tools.py` & `eva-shell-0.0.93/eva4_shell/tools.py`

 * *Files identical despite different names*

### Comparing `eva-shell-0.0.92/setup.py` & `eva-shell-0.0.93/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.0.92'
+__version__ = '0.0.93'
 
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(name='eva-shell',
```

