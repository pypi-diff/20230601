# Comparing `tmp/csv_scavenger-1.0.3.tar.gz` & `tmp/csv_scavenger-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_scavenger-1.0.3.tar", max compression
+gzip compressed data, was "csv_scavenger-1.0.4.tar", max compression
```

## Comparing `csv_scavenger-1.0.3.tar` & `csv_scavenger-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3030 2023-05-31 19:32:23.127800 csv_scavenger-1.0.3/csv-scavenger/scavenger.py
--rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.3/LICENSE
--rw-r--r--   0        0        0      542 2023-05-31 20:03:04.960811 csv_scavenger-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.3/README.md
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4026 2023-06-01 15:42:11.946420 csv_scavenger-1.0.4/csv-scavenger/scavenger.py
+-rw-r--r--   0        0        0     1094 2023-05-31 15:26:00.843242 csv_scavenger-1.0.4/LICENSE
+-rw-r--r--   0        0        0      542 2023-06-01 15:52:14.476265 csv_scavenger-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      663 2023-05-31 18:15:01.226065 csv_scavenger-1.0.4/README.md
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 csv_scavenger-1.0.4/PKG-INFO
```

### Comparing `csv_scavenger-1.0.3/csv-scavenger/scavenger.py` & `csv_scavenger-1.0.4/csv-scavenger/scavenger.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 
 def _determine_format(lines: list[str]) -> tuple[str, int]:
     formats: list[tuple[str, int]] = []
     step = len(lines) // 100 if len(lines) > 100 else 1
     for i, line in enumerate(lines):
         if i % step == 0:
             for delim in [";", ",", " ", "\t", "\n", "\r", "\r\n"]:
-                num_of_columns = len(line.strip().split(delim))
+                num_of_columns = len(
+                    tssplit(line.strip(), quote='"', delimiter=delim, escape="")  # type: ignore
+                )
                 if num_of_columns > 1:
                     formats.append((delim, num_of_columns))
     counter = Counter(formats)
     try:
         csv_format: tuple[str, int] = counter.most_common(1)[0][0]
     except IndexError:
         raise IndexError(
@@ -22,29 +24,46 @@
         )
     return csv_format
 
 
 def _determine_header_start_last(
     csv_format: tuple[str, int], lines: list[str]
 ) -> tuple[Optional[int], Optional[int], Optional[int]]:
-    header_line = None
-    last_line = None
+    header_line = "undefined"
+    last_line = "undefined"
+    first_line = "undefined"
 
     for i, line in enumerate(lines):
         num_of_columns = len(
             tssplit(line.strip(), quote='"', delimiter=csv_format[0], escape="")  # type: ignore
         )
-        if num_of_columns == csv_format[1] and header_line == None:
-            header_line = i
-        elif num_of_columns != csv_format[1] and header_line != None:
+        if num_of_columns == csv_format[1] and header_line == "undefined":
+            is_header = True
+            for item in tssplit(
+                line.strip(), quote='"', delimiter=csv_format[0], escape=""
+            ):
+                try:
+                    float(item)
+                    is_header = False
+                    break
+                except ValueError:
+                    pass
+            if is_header:
+                header_line = i
+                first_line = i + 1
+            else:
+                print("no header")
+                header_line = "none"
+                first_line = i
+        elif num_of_columns != csv_format[1] and header_line != "undefined":
             last_line = i
             break
-    if last_line == None:
+
+    if last_line == "undefined":
         last_line = len(lines)
-    first_line: Optional[int] = header_line + 1 if header_line != None else None
     return header_line, first_line, last_line
 
 
 def read_csv(file_path: str) -> pd.DataFrame:
     try:
         with open(file_path, "r") as file:
             lines = file.readlines()
@@ -52,25 +71,38 @@
         raise FileNotFoundError(f"File {file_path} not found.")
 
     csv_format = _determine_format(lines)
 
     header_row, data_start_row, data_end_row = _determine_header_start_last(
         csv_format, lines
     )
-
-    if header_row == None or data_start_row == None or data_end_row == None:
+    if (
+        header_row == "undefined"
+        or data_start_row == "undefined"
+        or data_end_row == "undefined"
+    ):
         raise ValueError("Could not determine header and data rows.")
 
-    data = pd.read_csv(  # type: ignore
-        file_path,
-        sep=csv_format[0],
-        skiprows=data_start_row - 1,
-        nrows=data_end_row - data_start_row,
-        engine="python",
-    )
+    if header_row == "none":
+        data = pd.read_csv(  # type: ignore
+            file_path,
+            sep=csv_format[0],
+            skiprows=data_start_row - 1,
+            nrows=data_end_row - data_start_row,
+            engine="python",
+            header=None,
+        )
+    else:
+        data = pd.read_csv(  # type: ignore
+            file_path,
+            sep=csv_format[0],
+            skiprows=data_start_row - 1,
+            nrows=data_end_row - data_start_row,
+            engine="python",
+        )
 
     if len(data) == 0:
         raise ValueError(
             f"CSV data is not in a recognized format. Detected delimiter is: {csv_format[0]}"
         )
 
     return data
@@ -78,8 +110,8 @@
 
 if __name__ == "__main__":
     data_people = read_csv("csv-scavenger/example_csvs/people.csv")
     data_faithful = read_csv("csv-scavenger/example_csvs/faithful.csv")
     data_orgs = read_csv("csv-scavenger/example_csvs/orgs.csv")
     data_health = read_csv("csv-scavenger/example_csvs/health.csv")
     data_multimeter = read_csv("csv-scavenger/example_csvs/multimeter.csv")
-    print(data_health)
+    print(data_multimeter)
```

### Comparing `csv_scavenger-1.0.3/LICENSE` & `csv_scavenger-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.3/pyproject.toml` & `csv_scavenger-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csv-scavenger"
-version = "1.0.3"
+version = "1.0.4"
 description = "CSV reader and parser with automatic detection of delimiter and start/end of data."
 authors = ["Gustave Coulombe <magikgus@gmail.com>"]
 readme = "README.md"
 packages = [{include = "scavenger.py", from = "csv-scavenger"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `csv_scavenger-1.0.3/README.md` & `csv_scavenger-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `csv_scavenger-1.0.3/PKG-INFO` & `csv_scavenger-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-scavenger
-Version: 1.0.3
+Version: 1.0.4
 Summary: CSV reader and parser with automatic detection of delimiter and start/end of data.
 Author: Gustave Coulombe
 Author-email: magikgus@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
```

