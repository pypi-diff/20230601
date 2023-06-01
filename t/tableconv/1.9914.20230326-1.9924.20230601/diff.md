# Comparing `tmp/tableconv-1.9914.20230326.tar.gz` & `tmp/tableconv-1.9924.20230601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableconv-1.9914.20230326.tar", last modified: Sun Mar 26 03:23:01 2023, max compression
+gzip compressed data, was "tableconv-1.9924.20230601.tar", last modified: Thu Jun  1 20:01:38 2023, max compression
```

## Comparing `tableconv-1.9914.20230326.tar` & `tableconv-1.9924.20230601.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.454336 tableconv-1.9914.20230326/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9914.20230326/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9914.20230326/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-03-26 03:23:01.454336 tableconv-1.9914.20230326/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9914.20230326/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2023-03-26 03:23:01.454336 tableconv-1.9914.20230326/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9914.20230326/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.450336 tableconv-1.9914.20230326/tableconv/
--rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       73 2023-03-26 03:22:57.000000 tableconv-1.9914.20230326/tableconv/__version__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.450336 tableconv-1.9914.20230326/tableconv/adapters/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9914.20230326/tableconv/adapters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.454336 tableconv-1.9914.20230326/tableconv/adapters/df/
--rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9914.20230326/tableconv/adapters/df/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/ascii.py
--rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/aws_athena.py
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/aws_dynamodb.py
--rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/aws_logs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9914.20230326/tableconv/adapters/df/example.py
--rw-rw-r--   0 john      (1000) john      (1000)     2517 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/file_adapter_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)    12680 2023-03-26 03:22:50.000000 tableconv-1.9914.20230326/tableconv/adapters/df/gsheets.py
--rw-rw-r--   0 john      (1000) john      (1000)      322 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/jira.py
--rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/json.py
--rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/nested_list.py
--rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9914.20230326/tableconv/adapters/df/numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     8873 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/pandas_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/python.py
--rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/rdbms.py
--rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/smart_sheet.py
--rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/sql_literal.py
--rw-rw-r--   0 john      (1000) john      (1000)     7472 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/sumo_logic.py
--rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/text_array.py
--rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/adapters/df/yaml.py
--rw-rw-r--   0 john      (1000) john      (1000)    15584 2023-03-26 03:19:10.000000 tableconv-1.9914.20230326/tableconv/core.py
--rw-r--r--   0 john      (1000) john      (1000)     2128 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     2911 2023-03-26 03:18:01.000000 tableconv-1.9914.20230326/tableconv/in_memory_query.py
--rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/interactive.py
--rw-rw-r--   0 john      (1000) john      (1000)    11199 2023-01-25 03:24:08.000000 tableconv-1.9914.20230326/tableconv/main.py
--rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/parse_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9914.20230326/tableconv/uri.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.450336 tableconv-1.9914.20230326/tableconv.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       66 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      243 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       27 2023-03-26 03:23:01.000000 tableconv-1.9914.20230326/tableconv.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-03-26 03:23:01.454336 tableconv-1.9914.20230326/tableconv_daemon/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9914.20230326/tableconv_daemon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9914.20230326/tableconv_daemon/main.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/
+-rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9924.20230601/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9924.20230601/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/
+-rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2023-06-01 20:00:30.000000 tableconv-1.9924.20230601/tableconv/__version__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/adapters/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9924.20230601/tableconv/adapters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv/adapters/df/
+-rw-rw-r--   0 john      (1000) john      (1000)      926 2023-01-27 19:23:04.000000 tableconv-1.9924.20230601/tableconv/adapters/df/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/ascii.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_athena.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_dynamodb.py
+-rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/aws_logs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9924.20230601/tableconv/adapters/df/example.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9924.20230601/tableconv/adapters/df/file_adapter_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12737 2023-05-02 00:16:20.000000 tableconv-1.9924.20230601/tableconv/adapters/df/gsheets.py
+-rw-rw-r--   0 john      (1000) john      (1000)      322 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/jira.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/nested_list.py
+-rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9924.20230601/tableconv/adapters/df/numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8873 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/pandas_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/python.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/rdbms.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/smart_sheet.py
+-rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/sql_literal.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7489 2023-05-03 19:19:16.000000 tableconv-1.9924.20230601/tableconv/adapters/df/sumo_logic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/text_array.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/adapters/df/yaml.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15584 2023-03-26 03:19:10.000000 tableconv-1.9924.20230601/tableconv/core.py
+-rw-r--r--   0 john      (1000) john      (1000)     2128 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2905 2023-06-01 19:58:47.000000 tableconv-1.9924.20230601/tableconv/in_memory_query.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/interactive.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11203 2023-05-05 19:10:26.000000 tableconv-1.9924.20230601/tableconv/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/parse_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9924.20230601/tableconv/uri.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1242 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       66 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      243 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       27 2023-06-01 20:01:38.000000 tableconv-1.9924.20230601/tableconv.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-06-01 20:01:38.705489 tableconv-1.9924.20230601/tableconv_daemon/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9924.20230601/tableconv_daemon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9924.20230601/tableconv_daemon/main.py
```

### Comparing `tableconv-1.9914.20230326/LICENSE` & `tableconv-1.9924.20230601/LICENSE`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/PKG-INFO` & `tableconv-1.9924.20230601/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9914.20230326
+Version: 1.9924.20230601
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9914.20230326/README.md` & `tableconv-1.9924.20230601/README.md`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/setup.py` & `tableconv-1.9924.20230601/setup.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/__init__.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/__init__.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/ascii.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/ascii.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/aws_athena.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/aws_athena.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/aws_dynamodb.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/aws_logs.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/aws_logs.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/base.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/base.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/file_adapter_mixin.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/file_adapter_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             try:
                 f.write(data)
             except BrokenPipeError:
                 if path == "/dev/fd/1":
                     # Ignore broken pipe error when outputting to stdout
                     return
                 raise
-        if data[-1] != "\n" and path == "/dev/fd/1" and sys.stdout.isatty():
+        if data and data[-1] != "\n" and path == "/dev/fd/1" and sys.stdout.isatty():
             print()
 
     @classmethod
     def load_text_data(cls, scheme: str, data: str, params: Dict[str, Any]) -> pd.DataFrame:
         raise NotImplementedError
 
     @classmethod
```

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/gsheets.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/gsheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
             .get(
                 spreadsheetId=spreadsheet_id,
                 range=f"'{sheet_name}'",
             )
             .execute()
         )
 
-        header = raw_data["values"][0]
-        num_columns = len(header)
+        num_columns = max(*[len(r) for r in  raw_data["values"]])
+        header = list_ljust(raw_data["values"][0], num_columns)
         values = [list_ljust(row, num_columns) for row in raw_data["values"][1:]]
         return pd.DataFrame(values, columns=header)
 
     @staticmethod
     def _create_spreadsheet(googlesheets, spreadsheet_name, first_sheet_name, columns, rows):
         sheet = {
             "properties": {
```

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/json.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/json.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/nested_list.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/nested_list.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/numbers.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/numbers.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/pandas_io.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/pandas_io.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/python.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/python.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/rdbms.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/rdbms.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/smart_sheet.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/smart_sheet.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/sql_literal.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/sql_literal.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/sumo_logic.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/sumo_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     search_job_id = search_job["id"]
 
     logger.info(f"Waiting for query to complete (job id: {search_job_id})")
     time.sleep((SUMO_API_RESULTS_POLLING_INTERVAL / 2).total_seconds())
     while True:
         status = sumo.search_job_status(search_job_id)
         if status["state"] != "GATHERING RESULTS":
-            assert status["state"] == "DONE GATHERING RESULTS"
+            assert status["state"] == "DONE GATHERING RESULTS", status["state"]
             break
         time.sleep(SUMO_API_RESULTS_POLLING_INTERVAL.total_seconds())
 
     message_count = status["messageCount"]
     logger.info(f"Downloading sumo results (message count: {message_count})")
 
     raw_results: List[Dict[str, Any]] = []
```

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/text_array.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/text_array.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/adapters/df/yaml.py` & `tableconv-1.9924.20230601/tableconv/adapters/df/yaml.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/core.py` & `tableconv-1.9924.20230601/tableconv/core.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/exceptions.py` & `tableconv-1.9924.20230601/tableconv/exceptions.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/in_memory_query.py` & `tableconv-1.9924.20230601/tableconv/in_memory_query.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         query = query.replace("transpose(data)", f'"{transposed_data_table_name}"')
         for table_name, df in dfs:
             if table_name == "data":
                 data_df = df
                 break
         transposed_data_df = data_df.transpose(copy=True).reset_index()
         dfs.append((transposed_data_table_name, transposed_data_df))
-    if re.search(r"\bunix\(", query):
-        for match in re.finditer(r"\bunix\((.+?)\)", query):
-            replacement = f"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds({match.group(1)}))"
-            query = query[: match.span()[0]] + replacement + query[match.span()[1] :]
+
+    query = re.sub(r"\bunix\((.+?)\)", r"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds(\1))", query)
+    query = re.sub(r"\biso8601\((.+?)\)", r"CAST(\1 AS TIMESTAMP)", query)
+    # re.sub(r"\biso8601\((.+?)\)", r"strptime(\1, '2023-04-01T18:36:01.200234+00:00')", query)
 
     return dfs, query
 
 
 def query_in_memory(dfs: List[Tuple[str, pd.DataFrame]], query: str) -> pd.DataFrame:
     """Warning: Has a side effect of mutating the dfs"""
     import duckdb
```

### Comparing `tableconv-1.9914.20230326/tableconv/interactive.py` & `tableconv-1.9924.20230601/tableconv/interactive.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/main.py` & `tableconv-1.9924.20230601/tableconv/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     set_up_logging()
     # Process arguments
     parser = NoExitArgParser(
         usage="%(prog)s SOURCE_URL [-q QUERY_SQL] [-o DEST_URL]",
         formatter_class=argparse.RawDescriptionHelpFormatter,  # Necessary for \n in epilog
         epilog=(
             f"supported url schemes:\n{get_supported_schemes_list_str()}\n\n"
-            "help & support:\n  https://github.com/personalcomputer/tableconv/issues"
+            "help & support:\n  https://github.com/personalcomputer/tableconv/issues/new"
         ),
         exit_on_error=False,
     )
     parser.add_argument("SOURCE_URL", type=str, help="Specify the data source URL.")
     parser.add_argument("-q", "-Q", "--query", dest="source_query", default=None, help="Query to run on the source. Even for non-SQL datasources (e.g. csv or json), SQL querying is still supported, try `SELECT * FROM data`.")  # noqa: E501
     parser.add_argument("-F", "--filter", dest="intermediate_filter_sql", default=None, help="Filter (i.e. transform) the input data using a SQL query operating on the dataset in memory using DuckDB SQL.")  # noqa: E501
     parser.add_argument("-o", "--dest", "--out", dest="DEST_URL", type=str, help="Specify the data destination URL. If this destination already exists, be aware that the default behavior is to overwrite.")  # noqa: E501
```

### Comparing `tableconv-1.9914.20230326/tableconv/parse_time.py` & `tableconv-1.9924.20230601/tableconv/parse_time.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv/uri.py` & `tableconv-1.9924.20230601/tableconv/uri.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv.egg-info/PKG-INFO` & `tableconv-1.9924.20230601/tableconv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9914.20230326
+Version: 1.9924.20230601
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tableconv-1.9914.20230326/tableconv.egg-info/SOURCES.txt` & `tableconv-1.9924.20230601/tableconv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tableconv-1.9914.20230326/tableconv_daemon/main.py` & `tableconv-1.9924.20230601/tableconv_daemon/main.py`

 * *Files identical despite different names*

