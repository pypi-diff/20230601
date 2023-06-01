# Comparing `tmp/AMDirT-1.4.3.tar.gz` & `tmp/AMDirT-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AMDirT-1.4.3.tar", last modified: Wed May  3 14:38:39 2023, max compression
+gzip compressed data, was "AMDirT-1.4.4.tar", last modified: Thu Jun  1 11:50:35 2023, max compression
```

## Comparing `AMDirT-1.4.3.tar` & `AMDirT-1.4.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/assets/tables.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/autofill/
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/autofill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/convert/
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/core/
--rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/core/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/core/ena.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/merge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/validate/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/validate/application/
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/validate/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/validate/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/validate/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/validate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT/viewer/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-05-03 14:38:33.000000 AMDirT-1.4.3/AMDirT/viewer/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:38:39.316974 AMDirT-1.4.3/AMDirT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 14:38:39.000000 AMDirT-1.4.3/AMDirT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-03 14:38:33.000000 AMDirT-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-03 14:38:39.316974 AMDirT-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-03 14:38:33.000000 AMDirT-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:38:39.316974 AMDirT-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-03 14:38:33.000000 AMDirT-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.642979 AMDirT-1.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/assets/tables.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/autofill/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/autofill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    15205 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/core/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/core/ena.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/merge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT/validate/application/
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/validate/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.642979 AMDirT-1.4.4/AMDirT/validate/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/validate/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/validate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.642979 AMDirT-1.4.4/AMDirT/viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-06-01 11:50:32.000000 AMDirT-1.4.4/AMDirT/viewer/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:50:35.638979 AMDirT-1.4.4/AMDirT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 11:50:35.000000 AMDirT-1.4.4/AMDirT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 11:50:32.000000 AMDirT-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-01 11:50:35.642979 AMDirT-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-01 11:50:32.000000 AMDirT-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:50:35.642979 AMDirT-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-01 11:50:32.000000 AMDirT-1.4.4/setup.py
```

### Comparing `AMDirT-1.4.3/AMDirT/assets/tables.json` & `AMDirT-1.4.4/AMDirT/assets/tables.json`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/autofill/__init__.py` & `AMDirT-1.4.4/AMDirT/autofill/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/cli.py` & `AMDirT-1.4.4/AMDirT/cli.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/convert/__init__.py` & `AMDirT-1.4.4/AMDirT/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/core/__init__.py` & `AMDirT-1.4.4/AMDirT/core/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/core/diff.py` & `AMDirT-1.4.4/AMDirT/core/diff.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/core/ena.py` & `AMDirT-1.4.4/AMDirT/core/ena.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/merge/__init__.py` & `AMDirT-1.4.4/AMDirT/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/validate/__init__.py` & `AMDirT-1.4.4/AMDirT/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/validate/application/__init__.py` & `AMDirT-1.4.4/AMDirT/validate/application/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/validate/domain/__init__.py` & `AMDirT-1.4.4/AMDirT/validate/domain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,23 +312,15 @@
         """Generate markdown output table for github display
 
         Returns:
             bool: True if dataset is valid
         Raises:
             SystemExit: If dataset is invalid
         """
-        df = pd.DataFrame(columns=["Error", "Source", "Column", "Row", "Message"])
-        for error in self.errors:
-            df = pd.concat(
-                [
-                    df,
-                    pd.Series(error.to_dict())
-                ],
-                ignore_index=True
-            )
-        if len(df) > 0:
+        if len(self.errors) > 0:
+            df = pd.concat([pd.Series(error.to_dict()).to_frame().transpose() for error in self.errors])
             raise SystemExit(
                 f"Invalid dataset `{self.dataset_name}`\n\n{df.to_markdown(index=False)}"
             )
         else:
             logger.info(f"{self.dataset_name} is valid")
             return True
```

### Comparing `AMDirT-1.4.3/AMDirT/validate/exceptions.py` & `AMDirT-1.4.4/AMDirT/validate/exceptions.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/viewer/__init__.py` & `AMDirT-1.4.4/AMDirT/viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT/viewer/streamlit.py` & `AMDirT-1.4.4/AMDirT/viewer/streamlit.py`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/AMDirT.egg-info/PKG-INFO` & `AMDirT-1.4.4/AMDirT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4.3
+Version: 1.4.4
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `AMDirT-1.4.3/AMDirT.egg-info/SOURCES.txt` & `AMDirT-1.4.4/AMDirT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/LICENSE` & `AMDirT-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/PKG-INFO` & `AMDirT-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AMDirT
-Version: 1.4.3
+Version: 1.4.4
 Summary: AMDirT: AncientMetagenomeDir Toolkit
 Home-page: https://github.com/SPAAM-community/AMDirT
 License: GNU-GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `AMDirT-1.4.3/README.md` & `AMDirT-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `AMDirT-1.4.3/setup.py` & `AMDirT-1.4.4/setup.py`

 * *Files identical despite different names*

