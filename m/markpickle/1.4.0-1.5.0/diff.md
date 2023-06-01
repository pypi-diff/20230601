# Comparing `tmp/markpickle-1.4.0.tar.gz` & `tmp/markpickle-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markpickle-1.4.0.tar", max compression
+gzip compressed data, was "markpickle-1.5.0.tar", max compression
```

## Comparing `markpickle-1.4.0.tar` & `markpickle-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1071 2023-05-31 01:40:36.109373 markpickle-1.4.0/LICENSE
--rw-r--r--   0        0        0     6119 2023-05-31 01:40:36.109373 markpickle-1.4.0/README.md
--rw-r--r--   0        0        0      574 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/__init__.py
--rw-r--r--   0        0        0     1397 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/__main__.py
--rw-r--r--   0        0        0     1697 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/atx_as_dictionary.py
--rw-r--r--   0        0        0     1543 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/binary_streams.py
--rw-r--r--   0        0        0       57 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/cli.py
--rw-r--r--   0        0        0     2298 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/config_class.py
--rw-r--r--   0        0        0    12845 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/deserialize.py
--rw-r--r--   0        0        0      412 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/meta.py
--rw-r--r--   0        0        0      568 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/mypy_types.py
--rw-r--r--   0        0        0       80 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/py.typed
--rw-r--r--   0        0        0     4817 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/python_to_tables.py
--rw-r--r--   0        0        0    14841 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/serialize.py
--rw-r--r--   0        0        0      737 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/simplify_types.py
--rw-r--r--   0        0        0     1032 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/split_file_code.py
--rw-r--r--   0        0        0     1252 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/third_party_tables.py
--rw-r--r--   0        0        0     1760 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/tool.py
--rw-r--r--   0        0        0      813 2023-05-31 01:40:36.109373 markpickle-1.4.0/markpickle/unicode_formatting.py
--rw-r--r--   0        0        0     3720 2023-05-31 01:40:36.109373 markpickle-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 markpickle-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-01 02:16:20.093850 markpickle-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6119 2023-06-01 02:16:20.093850 markpickle-1.5.0/README.md
+-rw-r--r--   0        0        0      574 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/__init__.py
+-rw-r--r--   0        0        0     1397 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/__main__.py
+-rw-r--r--   0        0        0     1697 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/atx_as_dictionary.py
+-rw-r--r--   0        0        0     1543 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/binary_streams.py
+-rw-r--r--   0        0        0       57 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/cli.py
+-rw-r--r--   0        0        0     2299 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/config_class.py
+-rw-r--r--   0        0        0    12988 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/deserialize.py
+-rw-r--r--   0        0        0      412 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/meta.py
+-rw-r--r--   0        0        0      568 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/mypy_types.py
+-rw-r--r--   0        0        0       80 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/py.typed
+-rw-r--r--   0        0        0     5412 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/python_to_tables.py
+-rw-r--r--   0        0        0    14985 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/serialize.py
+-rw-r--r--   0        0        0      737 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/simplify_types.py
+-rw-r--r--   0        0        0     1032 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/split_file_code.py
+-rw-r--r--   0        0        0     1252 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/third_party_tables.py
+-rw-r--r--   0        0        0     1760 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/tool.py
+-rw-r--r--   0        0        0      813 2023-06-01 02:16:20.097850 markpickle-1.5.0/markpickle/unicode_formatting.py
+-rw-r--r--   0        0        0     3720 2023-06-01 02:16:20.097850 markpickle-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 markpickle-1.5.0/PKG-INFO
```

### Comparing `markpickle-1.4.0/LICENSE` & `markpickle-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/README.md` & `markpickle-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/__init__.py` & `markpickle-1.5.0/markpickle/__init__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/__main__.py` & `markpickle-1.5.0/markpickle/__main__.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/atx_as_dictionary.py` & `markpickle-1.5.0/markpickle/atx_as_dictionary.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/binary_streams.py` & `markpickle-1.5.0/markpickle/binary_streams.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/config_class.py` & `markpickle-1.5.0/markpickle/config_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """What to write when a value is True or False"""
 
     none_values: list[str] = dataclasses.field(default_factory=lambda: ["None", "nil", "nil"])
     """What to write when a value is None"""
 
     empty_string_is: str = ""
 
-    tables_become_list_of_tuples = True
+    tables_become_list_of_tuples = False
     """If true, tables become list of tuples. If false, tables become list of dicts"""
 
     serialize_headers_are_dict_keys: bool = True
     """If true, use dict keys as headers when serializing a dict as a table"""
 
     serialize_dict_as_table: bool = False
     """If true, serialize a dict as a table if it is not a child of a dict"""
```

### Comparing `markpickle-1.4.0/markpickle/deserialize.py` & `markpickle-1.5.0/markpickle/deserialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,16 @@
             if token["children"][0]["type"] == "image":
                 return extract_bytes(token["children"][0]["src"], config)
 
             # Root scalar
             current_text_value: str = token["children"][0]["text"]
             if current_text_value.count("|") >= 2 and config.tables_become_list_of_tuples:
                 return python_to_tables.parse_table_with_regex(current_text_value)
+            elif current_text_value.count("|") >= 2:
+                return python_to_tables.parse_table_to_list_of_dict(current_text_value)
 
             return extract_scalar(current_text_value, config)
 
         elif (
             token["type"] == "paragraph"
             and token.get("children")
             and len(token["children"]) == 1
```

### Comparing `markpickle-1.4.0/markpickle/mypy_types.py` & `markpickle-1.5.0/markpickle/mypy_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/python_to_tables.py` & `markpickle-1.5.0/markpickle/python_to_tables.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,28 +71,45 @@
         table = header + separator + row
     else:
         table = row
 
     return f"{indentation}{table}"
 
 
+def parse_table_to_list_of_dict(md_table: str) -> list[dict[str, str]]:
+    """Treat tables as list of dictionaries"""
+    tuple_stuff = parse_table_with_regex(md_table)
+    headers = tuple_stuff[0]
+    rows = tuple_stuff[1:]
+    dict_stuff = []
+    for row in rows:
+        dict_row = {}
+        for column_id, column in enumerate(row):
+            dict_row[headers[column_id]] = column
+        dict_stuff.append(dict_row)
+    return dict_stuff
+
+
 def parse_table_with_regex(md_table: str) -> list[tuple[str, ...]]:
     """
-    Created by ChatGPT 3.5 Turbo model
+    Created by ChatGPT 3.5 Turbo model.
+
+    First element is headers, subsequent elements are rows.
     """
     rows = md_table.strip().split("\n")
     # Get the column names from the first row
     col_names = re.findall(r"\| *([^\|\n ]+) *", rows[0])
     num_cols = len(col_names)
     # Initialize the table data as a list of empty lists
     table_data = [[] for i in range(num_cols)]
     # Parse the remaining rows
     for row in rows[2:]:
         # Split the row into cells
-        cells = re.findall(r"\| *([^\|\n]+?) *", row)
+        # cells = re.findall(r"\| *([^\|\n]+?) *", row)
+        cells = [_.strip() for _ in row.strip().split("|")[1:-1]]
         # Check that the row has the correct number of cells
         if len(cells) != num_cols:
             raise ValueError(f"Row has {len(cells)} cells, but expected {num_cols}")
         # Add each cell to the appropriate column in the table data
         for i, cell in enumerate(cells):
             table_data[i].append(cell)
     # Combine the column names with the table data and return the result
```

### Comparing `markpickle-1.4.0/markpickle/serialize.py` & `markpickle-1.5.0/markpickle/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,19 +234,21 @@
         elif isinstance(item, list):
             if item and isinstance(item[0], dict):
                 if config.serialize_headers_are_dict_keys and indent == 0:
                     # headers dict keys. Can't nest.
                     header = f"{header_level * '#'} {key}\n"
                     builder.write(header)
                 else:
-                    header = f"{indent * ' '}{config.list_bullet_style} {key}\n"
+                    # Some markdown parsers treat 1 space indents as 0!
+                    header = f"{indent * '  '}{config.list_bullet_style} {key}\n"
                     builder.write(header)
                 python_to_tables.list_of_dict_to_markdown(builder, item, indent)
             else:
-                builder.write(f"{indent * ' '}{config.list_bullet_style} {key}\n")
+                # Some markdown parsers treat 1 space indents as 0!
+                builder.write(f"{indent * '  '}{config.list_bullet_style} {key}\n")
                 render_list(builder, item, config, indent + 1)
         elif isinstance(item, dict):
             builder.write(f"{'#' * header_level} {key}\n\n")
             if config.serialize_child_dict_as_table:
                 success = False
                 if config.serialize_tables_tabulate_style:
                     # pylint: disable=broad-exception-caught
```

### Comparing `markpickle-1.4.0/markpickle/simplify_types.py` & `markpickle-1.5.0/markpickle/simplify_types.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/split_file_code.py` & `markpickle-1.5.0/markpickle/split_file_code.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/third_party_tables.py` & `markpickle-1.5.0/markpickle/third_party_tables.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/tool.py` & `markpickle-1.5.0/markpickle/tool.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/markpickle/unicode_formatting.py` & `markpickle-1.5.0/markpickle/unicode_formatting.py`

 * *Files identical despite different names*

### Comparing `markpickle-1.4.0/pyproject.toml` & `markpickle-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markpickle"
-version = "1.4.0"
+version = "1.5.0"
 description = "Lossy python to markdown serializer"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["serializer", "deserializer", "markdown",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `markpickle-1.4.0/PKG-INFO` & `markpickle-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markpickle
-Version: 1.4.0
+Version: 1.5.0
 Summary: Lossy python to markdown serializer
 Home-page: https://github.com/matthewdeanmartin/markpickle
 License: MIT
 Keywords: serializer,deserializer,markdown
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Classifier: Development Status :: 3 - Alpha
```

