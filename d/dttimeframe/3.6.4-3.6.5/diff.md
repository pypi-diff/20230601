# Comparing `tmp/dttimeframe-3.6.4.tar.gz` & `tmp/dttimeframe-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dttimeframe-3.6.4.tar", last modified: Thu Jun  1 08:06:41 2023, max compression
+gzip compressed data, was "dttimeframe-3.6.5.tar", last modified: Thu Jun  1 09:12:27 2023, max compression
```

## Comparing `dttimeframe-3.6.4.tar` & `dttimeframe-3.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.416363 dttimeframe-3.6.4/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.4/LICENSE
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 08:06:41.411364 dttimeframe-3.6.4/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-04-12 08:03:29.000000 dttimeframe-3.6.4/README.md
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.339553 dttimeframe-3.6.4/dttimeframe/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.4/dttimeframe/__init__.py
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10696 2023-06-01 07:50:15.000000 dttimeframe-3.6.4/dttimeframe/timeFrame.py
-drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 08:06:41.393142 dttimeframe-3.6.4/dttimeframe.egg-info/
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/PKG-INFO
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/SOURCES.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/dependency_links.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-06-01 08:06:41.000000 dttimeframe-3.6.4/dttimeframe.egg-info/top_level.txt
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-06-01 08:06:41.417363 dttimeframe-3.6.4/setup.cfg
--rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-06-01 07:56:14.000000 dttimeframe-3.6.4/setup.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 09:12:27.955068 dttimeframe-3.6.5/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    35147 2023-01-11 07:08:21.000000 dttimeframe-3.6.5/LICENSE
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 09:12:27.950068 dttimeframe-3.6.5/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1853 2023-04-12 08:03:29.000000 dttimeframe-3.6.5/README.md
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 09:12:27.888096 dttimeframe-3.6.5/dttimeframe/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-03-29 08:33:59.000000 dttimeframe-3.6.5/dttimeframe/__init__.py
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)    10885 2023-06-01 09:05:28.000000 dttimeframe-3.6.5/dttimeframe/timeFrame.py
+drwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        0 2023-06-01 09:12:27.937068 dttimeframe-3.6.5/dttimeframe.egg-info/
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     2833 2023-06-01 09:12:27.000000 dttimeframe-3.6.5/dttimeframe.egg-info/PKG-INFO
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)      215 2023-06-01 09:12:27.000000 dttimeframe-3.6.5/dttimeframe.egg-info/SOURCES.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)        1 2023-06-01 09:12:27.000000 dttimeframe-3.6.5/dttimeframe.egg-info/dependency_links.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       12 2023-06-01 09:12:27.000000 dttimeframe-3.6.5/dttimeframe.egg-info/top_level.txt
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)       38 2023-06-01 09:12:27.956068 dttimeframe-3.6.5/setup.cfg
+-rwxrwxrwx   0 davidsoh  (1000) davidsoh  (1000)     1148 2023-06-01 09:10:12.000000 dttimeframe-3.6.5/setup.py
```

### Comparing `dttimeframe-3.6.4/LICENSE` & `dttimeframe-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.4/PKG-INFO` & `dttimeframe-3.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.4
+Version: 3.6.5
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.4/README.md` & `dttimeframe-3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `dttimeframe-3.6.4/dttimeframe/timeFrame.py` & `dttimeframe-3.6.5/dttimeframe/timeFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,25 @@
         else:
             self.append("")
             return open(self.name,mode)
     def clear(self) -> None: # clear content
         if self.name != "":
             with open(self.name,'w') as target_handle:
                     target_handle.write("")
+class recordHandle(fileHandle):
+    def __init__(self, handle:Any=json) -> None:
+        self.name = ""
+        self.stat = "init"
+        self.alt = None
+        self.handle = handle
     def load(self) -> dict:
-        return json.load(open(self.name)) if self.name != "" else {}
+        return self.handle.load(open(self.name)) if self.name != "" else {}
     def dump(self,target_dict:dict) -> None:
         with open(self.name,"w") as target_handle:
-            json.dump(target_dict,target_handle,indent=1)
+            self.handle.dump(target_dict,target_handle)
 #
 class tag:
     def __init__(self) -> None:
         #
         self.begin_time_str = ""
         self.delimiter_dict = {"date":"-","join":" ","time":":"}
         self.print_bool = True
@@ -49,15 +55,15 @@
         self.log.alt = sys.stdout  # type: ignore
         self.error = fileHandle()
         self.error.alt = sys.stderr  # type: ignore
         self.script = fileHandle()
         #
         # self.json_name = ""
         self.record_dict = dict()
-        self.extra = fileHandle()
+        self.extra = recordHandle()
     def clearFile(self) -> None:
         self.log.clear()
         self.error.clear()
         self.script.clear()
         self.extra.clear()
     def print(self,word_str:str,end:str="\n") -> None:
         log_list = [self.log,self.error]
@@ -178,30 +184,30 @@
         self.record(current_time_str,phrase_str)
         if self.extra.name != "":
             summary_dict = {}
             if Path(self.extra.name).exists():
                 summary_dict.update(self.extra.load())
             summary_dict.update({str(len(summary_dict)+x):y for x,y in self.record_dict.items()})
             self.extra.dump(dict_sort(summary_dict))
-    def indicator(self,input_str:str) -> bool:
+    def checkPoint(self,input_str:str) -> bool:
         if Path("stop.txt").exists():
             self.timeStamp(F"Manually skip, as 'stop.txt' existed, at [{input_str}]")
         else:
             self.timeStamp(F"{input_str}")
         return not Path("stop.txt").exists()
 #
 class detector:
-    def __init__(self,print_func:Any,call_func:Any) -> None:
+    def __init__(self,print_func:Any=print,call_func:Any=print,target_str:str="") -> None:
         self.target_str = ""
         self.doing_str = ""
         self.print = print_func
         self.call = call_func
         self.unlink = True
-    def func(self,input_str:str) -> None: # self.print and self.call
-        print(input_str)
+        if target_str != "":
+            self.do(target_str)
     def missing(self) -> bool:
         if Path(self.target_str).exists():
             self.print(F"NOTE: {self.target_str} existed")
             target_bool = False
         else:
             if Path(self.doing_str).exists():
                 if self.unlink:
```

### Comparing `dttimeframe-3.6.4/dttimeframe.egg-info/PKG-INFO` & `dttimeframe-3.6.5/dttimeframe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dttimeframe
-Version: 3.6.4
+Version: 3.6.5
 Summary: dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.
 Home-page: https://github.com/SotongDJ/dtTimeFrame
 Author: David Soh
 Author-email: ln@trth.nl
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dttimeframe-3.6.4/setup.py` & `dttimeframe-3.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name = "dttimeframe",
-    version = "3.6.4",
+    version = "3.6.5",
     author = "David Soh",
     author_email = "ln@trth.nl",
     description = "dtTimeFrame is a module that pack time track functions and subprocess call functions into one single class.",
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     url = "https://github.com/SotongDJ/dtTimeFrame",
     packages = ["dttimeframe"],
```

