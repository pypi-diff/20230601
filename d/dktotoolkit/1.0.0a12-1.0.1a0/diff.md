# Comparing `tmp/dktotoolkit-1.0.0a12.tar.gz` & `tmp/dktotoolkit-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-1.0.0a12.tar", last modified: Thu Jun  1 12:58:17 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.1a0.tar", last modified: Thu Jun  1 18:24:48 2023, max compression
```

## Comparing `dktotoolkit-1.0.0a12.tar` & `dktotoolkit-1.0.1a0.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 12:58:04.000000 dktotoolkit-1.0.0a12/LICENCE.txt
--rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/README.md
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.268872 dktotoolkit-1.0.0a12/src/dktotoolkit/
--rw-rw-rw-   0 root         (0) root         (0)     1602 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3162 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_loadenv.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/_replace_with_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py
--rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit/function/
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/function/_compatMode.py
--rw-rw-rw-   0 root         (0) root         (0)     2889 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py
--rw-rw-rw-   0 root         (0) root         (0)     4752 2023-06-01 12:31:22.000000 dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 12:58:17.272873 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6669 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      523 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 12:58:17.000000 dktotoolkit-1.0.0a12/src/dktotoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/dktotoolkit/
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/datestr.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/dotenv2clock.py
+-rw-rw-rw-   0 root         (0) root         (0)     4138 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/envvar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1321 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/dktotoolkit/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-01 18:24:48.000000 dktotoolkit-1.0.1a0/dktotoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-06-01 18:24:48.394357 dktotoolkit-1.0.1a0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-01 18:24:33.000000 dktotoolkit-1.0.1a0/setup.py
```

### Comparing `dktotoolkit-1.0.0a12/setup.cfg` & `dktotoolkit-1.0.1a0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 [metadata]
 name = dktotoolkit
-version = 1.0.0a12
 author = Pierre
 description = A little toolkit with fancy functions
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/module_toolkit
 project_urls = 
 	Source Code = https://framagit.org/discord-catho/module_toolkit
 keywords = dotenv, .env, toolkit, parse dates
 
 [options]
 python_requires = >=3.9, <4
-package_dir = 
-	=src
 packages = 
 	dktotoolkit
-	dktotoolkit.function
 
 [options.extras_require]
 doc = 
 	sphinx==6.2.1
 	sphinx-rtd-theme==1.2.1
 	myst-parser==1.0.0
 tests =
```

### Comparing `dktotoolkit-1.0.0a12/src/dktotoolkit/dict2obj.py` & `dktotoolkit-1.0.1a0/dktotoolkit/dict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-def _dict2obj(d=None, obj=None):
+def dict2obj(d=None, obj=None):
     """Convert nested Python dictionnary to object
 
 :author: geeksforgeeks.org
 
 :param dict d: input dictionnary
 :param obj: a class (could be empty)
     """
@@ -20,13 +20,13 @@
             pass
         #endClass
 
         obj = C()
     #endIf
 
     for k in d:
-        obj.__dict__[k] = _dict2obj(d[k])
+        obj.__dict__[k] = dict2obj(d[k])
     #endFor
 
     return obj
 
 #endDef
```

### Comparing `dktotoolkit-1.0.0a12/src/dktotoolkit/dotenv2clock.py` & `dktotoolkit-1.0.1a0/dktotoolkit/dotenv2clock.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.0a12/src/dktotoolkit/loadenv.py` & `dktotoolkit-1.0.1a0/dktotoolkit/envvar.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import os, sys
 
-def load(filename=None):
+def load_dotenv(filename:str="./.env", erase_variable:bool=False):
+    """Load .env file
 
-    if filename is None:
-        filename="./.env"
-    #endIf
+:param str filename: Path and name of the file (default: ./.env)
+:param bool erase_variable: Erase variable if already exists (default: False)
+"""
 
     sys.stdout.write(F"> Load environment file : {filename}\n")
 
     with open(filename,'r') as f:
         lines = f.readlines()
         for line in lines:
             l = line.split("\n")[0].split("#")[0].split("=")
             if len(l) > 1:
                 var = l[0].strip()
                 val = l[1].strip().replace(",",":").replace(";",":")
 
+                if os.environ.get(var, False) and not erase_variable:
+                    sys.stdout.write(F"load_env> {var} = {os.environ.get(var)} (already set, erase_variable)\n")
+                #endIf
+
                 sys.stdout.write(F"load_env> {var} = {val} : ")
                 if "\"" in val:
                     sys.stdout.write(F"warning : character \" in content (character removed)")
                     val = val.replace("\"","")
                 else:
                     sys.stdout.write(F"Done")
                 #endIf
@@ -34,86 +39,125 @@
     sys.stdout.write(F"\n")
 
     #TODO : ajouter valeurs par defaut si pas presentes !
 
 #endWith
 
 
-def getEnvironVar(varname:str):
-    var = os.environ.get(varname)
+def _castList(var:str, char:str):
 
-    def castList(var:str, char:str):
+    if "(" in var and ")" in var:
+        sublist=[""]
+        for e in var:
+            if e=="(":
+                sublist += ["",]
+            elif e == ")":
+                sublist += ["",]
+            else:
+                sublist[-1] += str(e)
+            #endIf
+        #endFor
 
-        if "(" in var and ")" in var:
-            sublist=[""]
-            for e in var:
-                if e=="(":
-                    sublist += ["",]
-                elif e == ")":
-                    sublist += ["",]
-                else:
-                    sublist[-1] += str(e)
-                #endIf
-            #endFor
+        tr_sb_list = []
+        for e in sublist:
+            if not e or e in ["", ":"]:
+                continue
+            #endIf
+            tr_sb_list += [castList(e, ":"),]
+        #endFor
 
-            tr_sb_list = []
-            for e in sublist:
-                if not e or e in ["", ":"]:
-                    continue
-                #endIf
-                tr_sb_list += [castList(e, ":"),]
-            #endFor
+        return tr_sb_list
+    #endIf
 
-            return tr_sb_list
-        #endIf
+    try:
 
-        try:
+        if isinstance(var, list) or isinstance(var, tuple):
+            return var
+        else:
+            L = [int(e.strip()) if e.strip().isdigit() else str(e.strip()) for e in var.split(char)]
+            return L
+        #endIf
+    except ValueError:
+        L = [str(e.strip()) for e in var.split(char)]
+        return L
+    except Exception as e:
+        print(e)
+        raise Exception
+    #endTry
+    return None
+#endDef
 
-            if isinstance(var, list) or isinstance(var, tuple):
-                return var
-            else:
-                L = [int(e.strip()) if e.strip().isdigit() else str(e.strip()) for e in var.split(char)]
-                return L
-            #endIf
-        except ValueError:
-             L = [str(e.strip()) for e in var.split(char)]
-             return L
-        except Exception as e:
-            print(e)
-            raise Exception
-        #endTry
-        return None
-    #endDef
+def getEnvironVar(varname:str):
+    var = os.environ.get(varname)
 
     if var is None :
         return None
     #endVar
     for char in [":",";",","]:  # separators
         if char in var:
 
-            L = castList(var, char)
+            L = _castList(var, char)
             if L is not None:
                 return L
             #endIf
         #endIf
     #endFor
 
-
     try:
         return int(var.strip())
     except ValueError:
         return str(var.strip())
 
     except Exception as e:
         print(e)
         raise Exception
     #endTry
 
 #endDef
 
 
+def getTimesReminder(dotenv_timevar="REMINDER", outdico=False):
+
+    # If no tzinfo is given then UTC is assumed.
+    tzone = ZoneInfo(getEnvironVar("TZONE", "Europe/Paris"))
+
+    tuples_dotenv = getEnvironVar(dotenv_timevar)
+    dico_out = {}
+
+    if tuples_dotenv is None:
+        return []
+    #endIf
+
+    for office, time in tuples_dotenv:
+        l_hourMinSec = ["", "", ""]
+        i = 0
+        for char in time:
+
+            if char.isdigit():
+                l_hourMinSec[i] = l_hourMinSec[i]+char
+                justchange=False
+            elif not justchange:
+                i += 1
+                justchange = True
+            #endIf
+        #endFor
+        l_hourMinSec = [int(e) if e else 0 for e in l_hourMinSec]
+        d_hourMinSec = {"hour":l_hourMinSec[0],"minute":l_hourMinSec[1],"second":l_hourMinSec[2]}
+
+        dico_out[office] = d_hourMinSec
+        dico_out[office]["time"] = datetime.time(**d_hourMinSec ,tzinfo=tzone)
+    #endFor
+
+    if outdico:
+        return dico_out
+    else:
+        return [v["time"] for k, v in dico_out.items()]
+    #endIf
+
+#endDef
+
 if __name__=="__main__":
     #print(getEnvironVar("PWD"))
     #print(getEnvironVar("PATH"))
-    fname="/home/pierre/Documents/Projets/bot_breviaire_v2/.env"
+    fname=".env"
     load(fname)
-    print(getEnvironVar("BRPIERE_BELLS"))
+    #print(getEnvironVar("BRPIERE_BELLS"))
```

### Comparing `dktotoolkit-1.0.0a12/src/dktotoolkit/parse_dates.py` & `dktotoolkit-1.0.1a0/dktotoolkit/datestr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,49 @@
 import sys
 import re
 from datetime import date, time, timedelta
+import traceback
 
+def parser_date(the_day:str="today", verbose:bool=True):
+    """Convert a date into the format YYYY-MM-DD
 
-def _parse_date(the_day=None):
-    the_day = the_day.lower()
+:param str the_day: The day (almost all formats, alors today, etc) (default: today)
+:param bool verbose: Verbose (default: True)
+"""
+    if isinstance(the_day, date):
+
+        return "{0:04d}-{1:02d}-{2:02d}".format(
+                int(the_day.year),
+                int(the_day.month),
+                int(the_day.day)
+        )
+
+    elif isinstance(the_day, str):
+
+        the_day = the_day.lower()
+
+    else:
+
+        raise parseError
+
+    #endIf
 
     if the_day is None or the_day in ["today", "aujourd_hui"]:
+
         today = date.today()
-        return "{0:04d}-{1:02d}-{2:02d}".format(int(today.year),int(today.month),int(today.day))
+        return "{0:04d}-{1:02d}-{2:02d}".format(
+                int(today.year),
+                int(today.month),
+                int(today.day)
+        )
+
     else:
-        return _str2date(date_string=the_day)
+
+        return _str2date(date_string=the_day, verbose=verbose)
+
     #endIf
 
     raise parseError
 #endDef
 
 
 def _parse_month(month_in):
@@ -48,19 +77,20 @@
         #endIf
     #endFor
 
     return month
 #endDef
 
 
-def _str2date(date_string:str=None, format_us:bool=None):
+def _str2date(date_string:str=None, format_us:bool=None, verbose:bool=True):
     """Convert an input date to a formated date
 
 :param str date_string: The date
 :param bool format_us: Set input format as YYYY MM DD
+:param bool verbose: Verbose (default: True)
 
 :return: date as format YYYY-MM-DD
 :rtypes: str
 """
     if date_string is None:
         return None
     #endIf
@@ -103,47 +133,63 @@
             pos_day_in=2
         #endIf
 
         # Recuperer le mois
         month = _parse_month(splitDate_in[1])
 
         if int(month) == 0: # si on a une inversion mois / jour (car mois > 12)
-            sys.stderr.write(f"pd> Warning : unknown month or inversion of month and days in {date_string} : {splitDate_in} ! I'll change month and day positions\n")
+            if verbose:
+                sys.stderr.write(f"pd> Warning : unknown month or inversion of month and days in {date_string} : {splitDate_in} ! I'll change month and day positions\n")
+            #endIf
             pos_month_in = pos_day_in
             pos_day_in = 1
 
             month = _parse_month(splitDate_in[pos_month_in])
 
             if int(month) == 0:
-                sys.stderr.write(f"pd> Warning : After one more test, unknown month in {date_string} : {splitDate_in} ! Delete month value\n")
+                if verbose:
+                    sys.stderr.write(f"pd> Warning : After one more test, unknown month in {date_string} : {splitDate_in} ! Delete month value\n")
+                #endIf
                 pos_day_in = pos_month_in
             #endIf
 
         #endIf
 
         day="{0:02d}".format(int(splitDate_in[pos_day_in]))
 
         return "{0:04d}-{1:02d}-{2:02d}".format(int(year),int(month),int(day))
 
     else:
 
         today = date.today()
         the_date = today
-
-        if date_string.lower() in ["hier","yesterday"]:
+        if date_string.lower() in ["aujourd'hui", "aujourd hui", "aujourdhui", "today"]:
+            pass
+        elif date_string.lower() in ["hier","yesterday"]:
             the_date = today - timedelta(days=1)
         elif date_string.lower() in ["avant-hier","before-yesterday"]:
             the_date = today - timedelta(days=2)
         elif date_string.lower() in ["demain","tomorrow"]:
             the_date = today + timedelta(days=1)
-        elif date_string.lower() in ["apres-demain", "après-demain","after-tomorrow"]:
+        elif date_string.lower() in ["apres demain", "après-demain", "apres-demain", "après-demain","after-tomorrow"]:
             the_date = today + timedelta(days=2)
         else:
-            sys.stderr.write("aelfRequest : Cas non implemente : {}\n".format(date_string))
+            t = traceback.format_list(traceback.extract_stack())
+            sys.stderr.write("".join(t))
+            sys.stderr.write("toolkit.datestr : Cas non implemente : {}\n".format(date_string))
+            return "00-00-0000"
         #endIf
 
-        return the_date
+        return _date2str(the_date)
     #endIf
 
     sys.stderr.write("Warning : unexpected case : I return a wrong date !\n")
     return "00-00-0000"
 #endDef
+
+def _date2str(date):
+    return "{0:04d}-{1:02d}-{2:02d}".format(
+                int(date.year),
+                int(date.month),
+                int(date.day)
+        )
+#endDef
```

