# Comparing `tmp/gdb_plus-6.3.0.tar.gz` & `tmp/gdb_plus-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdb_plus-6.3.0.tar", last modified: Thu Jun  1 20:45:46 2023, max compression
+gzip compressed data, was "gdb_plus-6.3.1.tar", last modified: Thu Jun  1 20:50:43 2023, max compression
```

## Comparing `gdb_plus-6.3.0.tar` & `gdb_plus-6.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.975666 gdb_plus-6.3.0/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.3.0/LICENSE
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:45:46.975336 gdb_plus-6.3.0/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13367 2023-06-01 20:44:31.000000 gdb_plus-6.3.0/README.md
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.971183 gdb_plus-6.3.0/gdb_plus/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    12472 2023-05-31 21:09:49.000000 gdb_plus-6.3.0/gdb_plus/Inner_Debugger.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-06-01 20:03:48.000000 gdb_plus-6.3.0/gdb_plus/__init__.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    99843 2023-06-01 20:01:57.000000 gdb_plus-6.3.0/gdb_plus/gdb_plus.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)    99228 2023-06-01 20:05:39.000000 gdb_plus-6.3.0/gdb_plus/gdb_plus_arm_dev.py
--rwxrwxrwx   0 edo       (1000) edo       (1000)     5125 2023-05-22 18:36:02.000000 gdb_plus-6.3.0/gdb_plus/utils.py
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.974073 gdb_plus-6.3.0/gdb_plus.egg-info/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 edo       (1000) edo       (1000)      321 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/requires.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-06-01 20:45:46.000000 gdb_plus-6.3.0/gdb_plus.egg-info/top_level.txt
--rwxrwxrwx   0 edo       (1000) edo       (1000)      657 2023-06-01 20:45:08.000000 gdb_plus-6.3.0/pyproject.toml
--rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-06-01 20:45:46.975764 gdb_plus-6.3.0/setup.cfg
-drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:45:46.974584 gdb_plus-6.3.0/tests/
--rwxrwxrwx   0 edo       (1000) edo       (1000)    20197 2023-06-01 16:55:57.000000 gdb_plus-6.3.0/tests/test.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.824262 gdb_plus-6.3.1/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    35148 2023-02-27 10:56:12.000000 gdb_plus-6.3.1/LICENSE
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:50:43.823979 gdb_plus-6.3.1/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13367 2023-06-01 20:44:31.000000 gdb_plus-6.3.1/README.md
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.819652 gdb_plus-6.3.1/gdb_plus/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    12472 2023-05-31 21:09:49.000000 gdb_plus-6.3.1/gdb_plus/Inner_Debugger.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      219 2023-06-01 20:03:48.000000 gdb_plus-6.3.1/gdb_plus/__init__.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    99855 2023-06-01 20:48:40.000000 gdb_plus-6.3.1/gdb_plus/gdb_plus.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    99228 2023-06-01 20:05:39.000000 gdb_plus-6.3.1/gdb_plus/gdb_plus_arm_dev.py
+-rwxrwxrwx   0 edo       (1000) edo       (1000)     5125 2023-05-22 18:36:02.000000 gdb_plus-6.3.1/gdb_plus/utils.py
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.822570 gdb_plus-6.3.1/gdb_plus.egg-info/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    13566 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      321 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        1 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       25 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/requires.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)        9 2023-06-01 20:50:43.000000 gdb_plus-6.3.1/gdb_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 edo       (1000) edo       (1000)      657 2023-06-01 20:50:24.000000 gdb_plus-6.3.1/pyproject.toml
+-rwxrwxrwx   0 edo       (1000) edo       (1000)       38 2023-06-01 20:50:43.824361 gdb_plus-6.3.1/setup.cfg
+drwxrwxrwx   0 edo       (1000) edo       (1000)        0 2023-06-01 20:50:43.823163 gdb_plus-6.3.1/tests/
+-rwxrwxrwx   0 edo       (1000) edo       (1000)    20197 2023-06-01 16:55:57.000000 gdb_plus-6.3.1/tests/test.py
```

### Comparing `gdb_plus-6.3.0/LICENSE` & `gdb_plus-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.0/PKG-INFO` & `gdb_plus-6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb_plus
-Version: 6.3.0
+Version: 6.3.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
```

### Comparing `gdb_plus-6.3.0/README.md` & `gdb_plus-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.0/gdb_plus/Inner_Debugger.py` & `gdb_plus-6.3.1/gdb_plus/Inner_Debugger.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.0/gdb_plus/gdb_plus.py` & `gdb_plus-6.3.1/gdb_plus/gdb_plus.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 from time import sleep
 from functools import partial
 from capstone import Cs, CS_ARCH_X86
 from threading import Event
 from queue import Queue
 from gdb_plus.utils import Arguments, user_regs_struct, context, MyEvent, Breakpoint
-from libdebug import Debugger as lib_Debugger
 #import logging
 
 #log = logging.getLogger("gdb_plus")
 
 RET = b"\xc3"
 DEBUG_OFF = "Debug is off, commands won't be executed"
 # Yah, there should be a way to handle the logs and hide those from the library, but will look into it another day.
@@ -268,14 +267,15 @@
             self.__setup_gdb()
             # I must get back before setting the breakpoints otherwise I may overwrite them
             self.write(address, backup)
             self.jump(address)
             for address in self.breakpoints:
                 self.__breakpoint_gdb(address)
         elif libdebug:
+            from libdebug import Debugger as lib_Debugger
             # Disable hook stop
             self.gdb.events.exited.disconnect(self.__exit_handler)
             self.detach()
             assert self.libdebug is None
             log.debug("migrating to libdebug")
             self.gdb = None
             self.libdebug = lib_Debugger()
```

### Comparing `gdb_plus-6.3.0/gdb_plus/gdb_plus_arm_dev.py` & `gdb_plus-6.3.1/gdb_plus/gdb_plus_arm_dev.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.0/gdb_plus/utils.py` & `gdb_plus-6.3.1/gdb_plus/utils.py`

 * *Files identical despite different names*

### Comparing `gdb_plus-6.3.0/gdb_plus.egg-info/PKG-INFO` & `gdb_plus-6.3.1/gdb_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdb-plus
-Version: 6.3.0
+Version: 6.3.1
 Summary: Python library to automate gdb debugging
 Author: Edoardo
 Project-URL: Homepage, https://github.com/Angelo942/pydbg
 Project-URL: Bug Tracker, https://github.com/Angelo942/pydbg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
```

### Comparing `gdb_plus-6.3.0/pyproject.toml` & `gdb_plus-6.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools",
     "wheel",
 ]
 
 [project]
 name = "gdb_plus"
 description = "Python library to automate gdb debugging"
-version = "6.3.0"
+version = "6.3.1"
 authors = [{name = "Edoardo"}]
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "pwntools>=4.5.0",
     "capstone",
 ]
```

### Comparing `gdb_plus-6.3.0/tests/test.py` & `gdb_plus-6.3.1/tests/test.py`

 * *Files identical despite different names*

