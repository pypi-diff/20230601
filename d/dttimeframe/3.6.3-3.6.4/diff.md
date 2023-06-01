# Comparing `tmp/dttimeframe-3.6.3.tar.gz` & `tmp/dttimeframe-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dttimeframe-3.6.3.tar", last modified: Wed Apr 12 07:21:03 2023, max compression
+gzip compressed data, was "dttimeframe-3.6.4.tar", last modified: Thu Jun  1 08:06:41 2023, max compression
```

## Comparing `dttimeframe-3.6.3.tar` & `dttimeframe-3.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:03.012568 dttimeframe-3.6.3/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.3/LICENSE
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-04-12 07:21:03.009134 dttimeframe-3.6.3/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-04-12 07:11:15.000000 dttimeframe-3.6.3/README.md
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:02.949689 dttimeframe-3.6.3/dttimeframe/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.3/dttimeframe/__init__.py
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10515 2023-03-29 08:33:59.000000 dttimeframe-3.6.3/dttimeframe/timeFrame.py
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-04-12 07:21:02.997727 dttimeframe-3.6.3/dttimeframe.egg-info/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-04-12 07:21:02.000000 dttimeframe-3.6.3/dttimeframe.egg-info/top_level.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-04-12 07:21:03.013885 dttimeframe-3.6.3/setup.cfg
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-04-12 07:13:41.000000 dttimeframe-3.6.3/setup.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.416363 dttimeframe-3.6.4/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.4/LICENSE
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 08:06:41.411364 dttimeframe-3.6.4/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-04-12 08:03:29.000000 dttimeframe-3.6.4/README.md
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.339553 dttimeframe-3.6.4/dttimeframe/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.4/dttimeframe/__init__.py
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10696 2023-06-01 07:50:15.000000 dttimeframe-3.6.4/dttimeframe/timeFrame.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.393142 dttimeframe-3.6.4/dttimeframe.egg-info/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/top_level.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-06-01 08:06:41.417363 dttimeframe-3.6.4/setup.cfg
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-06-01 07:56:14.000000 dttimeframe-3.6.4/setup.py
```

### Comparing `dttimeframe-3.6.3/LICENSE` & `dttimeframe-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.3/PKG-INFO` & `dttimeframe-3.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.3
+Version: 3.6.4
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.3/README.md` & `dttimeframe-3.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.3/dttimeframe/timeFrame.py` & `dttimeframe-3.6.4/dttimeframe/timeFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import datetime
 import json
 import math
-import pathlib
 import sys
 import time
+from pathlib import Path
 from subprocess import call
 from typing import Any
 
 #
 class fileHandle:
     def __init__(self) -> None:
         self.name = ""
@@ -174,48 +174,53 @@
         end_phrase_str = "Finished on [{}]\n     Total time: {}"
         convert_time_str = self.convertTime(current=current_time_str)
         phrase_str = end_phrase_str.format(convert_time_str,totalTimeStr)
         self.print(phrase_str)
         self.record(current_time_str,phrase_str)
         if self.extra.name != "":
             summary_dict = {}
-            if pathlib.Path(self.extra.name).exists():
+            if Path(self.extra.name).exists():
                 summary_dict.update(self.extra.load())
-            entry_prefix_str = "[{}] ".format(len(summary_dict))
-            summary_dict.update({F"{entry_prefix_str}{x}":y for x,y in self.record_dict.items()})
-            self.extra.dump(summary_dict)
+            summary_dict.update({str(len(summary_dict)+x):y for x,y in self.record_dict.items()})
+            self.extra.dump(dict_sort(summary_dict))
+    def indicator(self,input_str:str) -> bool:
+        if Path("stop.txt").exists():
+            self.timeStamp(F"Manually skip, as 'stop.txt' existed, at [{input_str}]")
+        else:
+            self.timeStamp(F"{input_str}")
+        return not Path("stop.txt").exists()
 #
 class detector:
     def __init__(self,print_func:Any,call_func:Any) -> None:
         self.target_str = ""
         self.doing_str = ""
         self.print = print_func
         self.call = call_func
         self.unlink = True
     def func(self,input_str:str) -> None: # self.print and self.call
         print(input_str)
     def missing(self) -> bool:
-        if pathlib.Path(self.target_str).exists():
+        if Path(self.target_str).exists():
             self.print(F"NOTE: {self.target_str} existed")
             target_bool = False
         else:
-            if pathlib.Path(self.doing_str).exists():
+            if Path(self.doing_str).exists():
                 if self.unlink:
-                    pathlib.Path(self.doing_str).unlink()
+                    Path(self.doing_str).unlink()
                     self.print(F"NOTE: {self.doing_str} removed")
                     target_bool = True
                 else:
                     self.print(F"NOTE: {self.doing_str} keep and skip")
                     target_bool = False
             else:
                 target_bool = True
         return target_bool
     def do(self,target_str:str) -> None:
         self.target_str = target_str
-        self.doing_str = "{}/{}".format(pathlib.Path(target_str).parent,"doing-"+pathlib.Path(target_str).name)
+        self.doing_str = "{}/{}".format(Path(target_str).parent,"doing-"+Path(target_str).name)
     def done(self) -> None:
         self.print(F"NOTE: {self.doing_str} done")
         self.call(F"mv -v {self.doing_str} {self.target_str}")
 #
 class paginator:
     def __init__(self,input_list:list,split_num:int=5) -> None:
         self.parent_list = input_list
```

### Comparing `dttimeframe-3.6.3/dttimeframe.egg-info/PKG-INFO` & `dttimeframe-3.6.4/dttimeframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.3
+Version: 3.6.4
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.3/setup.py` & `dttimeframe-3.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = "dttimeframe",
-    version = "3.6.3",
+    version = "3.6.4",
     author = "David Soh",
     author_email = "ln@trth.nl",
     description = "dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.",
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     url = "https://github.com/SotongDJ/dtTimeFrame",
     packages = ["dttimeframe"],
```

