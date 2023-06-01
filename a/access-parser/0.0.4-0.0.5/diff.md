# Comparing `tmp/access_parser-0.0.4.tar.gz` & `tmp/access_parser-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/access_parser-0.0.4.tar", last modified: Mon Jul 12 13:07:40 2021, max compression
+gzip compressed data, was "access_parser-0.0.5.tar", last modified: Thu Jun  1 07:12:27 2023, max compression
```

## Comparing `access_parser-0.0.4.tar` & `access_parser-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 urikatz    (501) staff       (20)        0 2021-07-12 13:07:40.000000 access_parser-0.0.4/
--rw-r--r--   0 urikatz    (501) staff       (20)     2387 2021-07-12 13:07:40.000000 access_parser-0.0.4/PKG-INFO
-drwxr-xr-x   0 urikatz    (501) staff       (20)        0 2021-07-12 13:07:40.000000 access_parser-0.0.4/access_parser/
--rw-r--r--   0 urikatz    (501) staff       (20)    23064 2021-07-12 13:00:45.000000 access_parser-0.0.4/access_parser/access_parser.py
--rw-r--r--   0 urikatz    (501) staff       (20)       53 2021-05-09 09:35:39.000000 access_parser-0.0.4/access_parser/__init__.py
--rw-r--r--   0 urikatz    (501) staff       (20)     7943 2021-07-12 13:00:45.000000 access_parser-0.0.4/access_parser/parsing_primitives.py
--rw-r--r--   0 urikatz    (501) staff       (20)     3928 2021-07-12 13:00:45.000000 access_parser-0.0.4/access_parser/utils.py
-drwxr-xr-x   0 urikatz    (501) staff       (20)        0 2021-07-12 13:07:40.000000 access_parser-0.0.4/access_parser.egg-info/
--rw-r--r--   0 urikatz    (501) staff       (20)     2387 2021-07-12 13:07:39.000000 access_parser-0.0.4/access_parser.egg-info/PKG-INFO
--rw-r--r--   0 urikatz    (501) staff       (20)      318 2021-07-12 13:07:39.000000 access_parser-0.0.4/access_parser.egg-info/SOURCES.txt
--rw-r--r--   0 urikatz    (501) staff       (20)       19 2021-07-12 13:07:39.000000 access_parser-0.0.4/access_parser.egg-info/requires.txt
--rw-r--r--   0 urikatz    (501) staff       (20)       14 2021-07-12 13:07:39.000000 access_parser-0.0.4/access_parser.egg-info/top_level.txt
--rw-r--r--   0 urikatz    (501) staff       (20)        1 2021-07-12 13:07:39.000000 access_parser-0.0.4/access_parser.egg-info/dependency_links.txt
--rw-r--r--   0 urikatz    (501) staff       (20)     1539 2021-05-09 09:35:39.000000 access_parser-0.0.4/README.md
--rw-r--r--   0 urikatz    (501) staff       (20)      745 2021-07-12 13:02:17.000000 access_parser-0.0.4/setup.py
--rw-r--r--   0 urikatz    (501) staff       (20)       38 2021-07-12 13:07:40.000000 access_parser-0.0.4/setup.cfg
+drwxrwxr-x   0 uri       (1000) uri       (1000)        0 2023-06-01 07:12:27.416728 access_parser-0.0.5/
+-rw-rw-r--   0 uri       (1000) uri       (1000)    11357 2023-06-01 07:11:52.000000 access_parser-0.0.5/LICENSE
+-rw-rw-r--   0 uri       (1000) uri       (1000)     1927 2023-06-01 07:12:27.412728 access_parser-0.0.5/PKG-INFO
+-rw-rw-r--   0 uri       (1000) uri       (1000)     1473 2023-06-01 07:11:52.000000 access_parser-0.0.5/README.md
+drwxrwxr-x   0 uri       (1000) uri       (1000)        0 2023-06-01 07:12:27.412728 access_parser-0.0.5/access_parser/
+-rw-rw-r--   0 uri       (1000) uri       (1000)       53 2023-06-01 07:11:52.000000 access_parser-0.0.5/access_parser/__init__.py
+-rw-rw-r--   0 uri       (1000) uri       (1000)    27350 2023-06-01 07:11:52.000000 access_parser-0.0.5/access_parser/access_parser.py
+-rw-rw-r--   0 uri       (1000) uri       (1000)     9070 2023-06-01 07:11:52.000000 access_parser-0.0.5/access_parser/parsing_primitives.py
+-rw-rw-r--   0 uri       (1000) uri       (1000)     6941 2023-06-01 07:11:52.000000 access_parser-0.0.5/access_parser/utils.py
+drwxrwxr-x   0 uri       (1000) uri       (1000)        0 2023-06-01 07:12:27.412728 access_parser-0.0.5/access_parser.egg-info/
+-rw-rw-r--   0 uri       (1000) uri       (1000)     1927 2023-06-01 07:12:27.000000 access_parser-0.0.5/access_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 uri       (1000) uri       (1000)      326 2023-06-01 07:12:27.000000 access_parser-0.0.5/access_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 uri       (1000) uri       (1000)        1 2023-06-01 07:12:27.000000 access_parser-0.0.5/access_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 uri       (1000) uri       (1000)       19 2023-06-01 07:12:27.000000 access_parser-0.0.5/access_parser.egg-info/requires.txt
+-rw-rw-r--   0 uri       (1000) uri       (1000)       14 2023-06-01 07:12:27.000000 access_parser-0.0.5/access_parser.egg-info/top_level.txt
+-rw-rw-r--   0 uri       (1000) uri       (1000)       38 2023-06-01 07:12:27.416728 access_parser-0.0.5/setup.cfg
+-rw-rw-r--   0 uri       (1000) uri       (1000)      745 2023-06-01 07:11:52.000000 access_parser-0.0.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `access_parser-0.0.4/PKG-INFO` & `access_parser-0.0.5/access_parser.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 Metadata-Version: 2.1
-Name: access_parser
-Version: 0.0.4
+Name: access-parser
+Version: 0.0.5
 Summary: Access database (*.mdb, *.accdb) parser
 Home-page: https://github.com/ClarotyICS/access_parser
 Author: Uri Katz
 Author-email: uri.k@claroty.com
-License: UNKNOWN
-Description: # AccessDB Parser
-        Microsoft Access (.mdb / .accdb) database files parser. The parsing logic is fully written in python and works without any external binary dependencies.
-        
-        # Installing
-        Use pip: `pip install access-parser`
-        
-        Or install manually:
-        ```bash
-        git clone https://github.com/ClarotyICS/access_parser.git
-        cd access_parser
-        python3 setup.py install
-        ```
-        
-        # Demo
-        [![asciicast](https://asciinema.org/a/345445.svg)](https://asciinema.org/a/345445)
-        
-        # Usage Example
-        ```python
-        from access_parser import AccessParser
-        
-        # .mdb or .accdb file
-        db = AccessParser("/path/to/mdb/file.mdb")
-        
-        # Print DB tables
-        print(db.catalog)
-        
-        # Tables are stored as defaultdict(list) -- table[column][row_index]
-        table = db.parse_table("table_name")
-        
-        # Pretty print all tables
-        db.print_database()
-        
-        ```
-        
-        ### Known Issues
-        * OLE fields are currently not supported
-        * Only a subset of memo fields are parsed
-        
-        This library was tested on a limited subset of database files. Due to the differences between database versions and the complexity of the parsing we expect to find more parsing edge-cases.
-        
-        To help us resolve issues faster please provide as much data as you can when opening an issue - DB file if possible and full trace including log messages.
-         
-         
-        ### Thanks
-        * This library was made possible by the great work by mdb-tools. The logic in this library heavily relies on the excellent documentation they have https://github.com/brianb/mdbtools
-        * Huge thanks to Mashav Sapir for the help debugging, CRing and contributing to this project https://github.com/mashavs
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AccessDB Parser (Pure Python)
+Microsoft Access (.mdb / .accdb) database files parser. The parsing logic is fully written in python and works without any external binary dependencies.
+
+# Installing
+Use pip: `pip install access-parser`
+
+Or install manually:
+```bash
+git clone https://github.com/ClarotyICS/access_parser.git
+cd access_parser
+python3 setup.py install
+```
+
+# Demo
+[![asciicast](https://asciinema.org/a/345445.svg)](https://asciinema.org/a/345445)
+
+# Usage Example
+```python
+from access_parser import AccessParser
+
+# .mdb or .accdb file
+db = AccessParser("/path/to/mdb/file.mdb")
+
+# Print DB tables
+print(db.catalog)
+
+# Tables are stored as defaultdict(list) -- table[column][row_index]
+table = db.parse_table("table_name")
+
+# Pretty print all tables
+db.print_database()
+
+```
+
+### Known Issues
+* 
+
+This library was tested on a limited subset of database files. Due to the differences between database versions and the complexity of the parsing we expect to find more parsing edge-cases.
+
+To help us resolve issues faster please provide as much data as you can when opening an issue - DB file if possible and full trace including log messages.
+ 
+ 
+### Thanks
+* This library was made possible by the great work by mdb-tools. The logic in this library heavily relies on the excellent documentation they have https://github.com/brianb/mdbtools
+* Huge thanks to Mashav Sapir for the help debugging, CRing and contributing to this project https://github.com/mashavs
```

### Comparing `access_parser-0.0.4/access_parser/access_parser.py` & `access_parser-0.0.5/access_parser/access_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import struct
 from collections import defaultdict
 
 from construct import ConstructError
 from tabulate import tabulate
 
 from .parsing_primitives import parse_relative_object_metadata_struct, parse_table_head, parse_data_page_header, \
-    ACCESSHEADER, MEMO, parse_table_data, TDEF_HEADER
+    ACCESSHEADER, MEMO, parse_table_data, TDEF_HEADER, LVPROP
 from .utils import categorize_pages, parse_type, TYPE_MEMO, TYPE_TEXT, TYPE_BOOLEAN, read_db_file, numeric_to_string, \
-    TYPE_96_bit_17_BYTES
+    TYPE_96_bit_17_BYTES, TYPE_OLE
 
 # Page sizes
 PAGE_SIZE_V3 = 0x800
 PAGE_SIZE_V4 = 0x1000
 
 # Versions
 VERSION_3 = 0x00
@@ -39,14 +39,26 @@
 class AccessParser(object):
     def __init__(self, db_path):
         self.db_data = read_db_file(db_path)
         self._parse_file_header(self.db_data)
         self._table_defs, self._data_pages, self._all_pages = categorize_pages(self.db_data, self.page_size)
         self._tables_with_data = self._link_tables_to_data()
         self.catalog = self._parse_catalog()
+        self.extra_props = self.parse_msys_table()
+
+    def parse_msys_table(self):
+        """The MSysObjects contains extra metadata about tables and columns, like the Format of money field types """
+        msys_table = self.parse_table("MSysObjects")
+        if not msys_table:
+            return None
+        if not msys_table.get('Name') or not msys_table.get('LvProp'):
+            return []
+        table_to_lval_memo = {key: self.parse_lvprop(value) for key, value in zip(msys_table['Name'],
+                                                                                  msys_table['LvProp']) if value}
+        return table_to_lval_memo
 
     def _parse_file_header(self, db_data):
         """
         Parse the basic file header and determine the Access DB version based on the parsing results.
         :param db_data: db file data
         """
         try:
@@ -99,24 +111,54 @@
         :return: dict {table : offset}
         """
         catalog_page = self._tables_with_data[2 * self.page_size]
         access_table = AccessTable(catalog_page, self.version, self.page_size, self._data_pages, self._table_defs)
         catalog = access_table.parse()
         tables_mapping = {}
         for i, table_name in enumerate(catalog['Name']):
+            # We need the MSysObjects table for metadata so exclude it from the system table filter.
+            if table_name == "MSysObjects":
+                tables_mapping[table_name] = catalog['Id'][i]
             # Visible user tables are type 1
             table_type = 1
             if catalog["Type"][i] == table_type:
                 # Don't parse system tables
                 if not catalog["Flags"][i] in SYSTEM_TABLE_FLAGS:
                     tables_mapping[table_name] = catalog['Id'][i]
                 else:
                     logging.debug(f"Not parsing system table - {table_name}")
         return tables_mapping
 
+    def parse_lvprop(self, lvprop_raw):
+        try:
+            parsed = LVPROP.parse(lvprop_raw)
+        except ConstructError:
+            return None
+        if not parsed.get("chunks"):
+            return None
+        table_names = [x.name for x in parsed.chunks[0].data.names]
+        # Chunk type 0 does not have a column name, so we cannot link it to a column
+        chunk_type_one = [x for x in parsed.chunks if x.chunk_type == 1]
+        reconstructed_column_data = {}
+        for chunk in chunk_type_one:
+            if not chunk.data.column_name:
+                logging.error("Error while parsing MSysObjects table chunk.")
+                continue
+            data_values = {}
+            for dv in chunk.data.data:
+                val = parse_type(dv.type, dv.actual_data, version=self.version)
+                try:
+                    name = table_names[dv.name_index]
+                    data_values[name] = val
+                except IndexError:
+                    logging.error("Error while parsing MSysObjects table chunk.")
+                    continue
+            reconstructed_column_data[chunk.data.column_name] = data_values
+        return reconstructed_column_data
+
     def parse_table(self, table_name):
         """
         Parse a table from the db.
         tables names are in self.catalog
         :return defaultdict(list) with the parsed table -- table[column][row_index]
         """
         table_offset = self.catalog.get(table_name)
@@ -129,34 +171,41 @@
             table_def = self._table_defs.get(table_offset)
             if table_def:
                 table = TableObj(offset=table_offset, val=table_def)
                 logging.info(f"Table {table_name} has no data")
             else:
                 logging.error(f"Could not find table {table_name} offset {table_offset}")
                 return
-        access_table = AccessTable(table, self.version, self.page_size, self._data_pages, self._table_defs)
+
+        # Try to get extra metadata for the table if it exists in the MSysObjects table
+        props = None
+        if table_name != "MSysObjects" and table_name in self.extra_props:
+            props = self.extra_props[table_name]
+
+        access_table = AccessTable(table, self.version, self.page_size, self._data_pages, self._table_defs, props)
         return access_table.parse()
 
     def print_database(self):
         """
         Print data from all database tables
         """
         table_names = self.catalog
         for table_name in table_names:
             table = self.parse_table(table_name)
             if not table:
                 continue
             print(f'TABLE NAME: {table_name}\r\n')
-            print(tabulate(table, headers="keys"))
+            print(tabulate(table, headers="keys", disable_numparse=True))
             print('\r\n\r\n\r\n\r\n')
 
 
 class AccessTable(object):
-    def __init__(self, table, version, page_size, data_pages, table_defs):
+    def __init__(self, table, version, page_size, data_pages, table_defs, props=None):
         self.version = version
+        self.props = props
         self.page_size = page_size
         self._data_pages = data_pages
         self._table_defs = table_defs
         self.table = table
         self.parsed_table = defaultdict(list)
         self.columns, self.table_header = self._get_table_columns()
 
@@ -244,38 +293,46 @@
             self._parse_fixed_length_data(record, column, null_table)
         if relative_records_column_map:
             relative_records_column_map = dict(sorted(relative_records_column_map.items()))
             metadata = self._parse_dynamic_length_records_metadata(reverse_record, original_record,
                                                                    null_table_len)
             if not metadata:
                 return
-            self._parse_dynamic_length_data(original_record, metadata, relative_records_column_map)
+            if metadata.variable_length_field_offsets:
+                self._parse_dynamic_length_data(original_record, metadata, relative_records_column_map, null_table)
 
     def _parse_fixed_length_data(self, original_record, column, null_table):
         """
         Parse fixed-length data from record
         :param original_record: unmodified record
         :param column: column this data belongs to
         :param null_table: null table of the row
         """
         column_name = column.col_name_str
+        # The null table indicates null values in the row.
+        # The only exception is BOOL fields which are encoded in the null table
+        has_value = True
+        if column.column_id > len(null_table):
+            logging.warning("Invalid null table. Bool values may be wrong, deleted values may be shown in the db.")
+            if column.type == TYPE_BOOLEAN:
+                has_value = None
+        else:
+            has_value = null_table[column.column_id]
         # Boolean fields are encoded in the null table
         if column.type == TYPE_BOOLEAN:
-            if column.column_id > len(null_table):
-                logging.error(f"Failed to parse bool field, Column not found in null_table column: {column_name} ,"
-                              f" column id: {column.column_id} , null_table: {null_table}")
-                return
-
-            parsed_type = null_table[column.column_id]
+            parsed_type = has_value
         else:
             if column.fixed_offset > len(original_record):
                 logging.error(f"Column offset is bigger than the length of the record {column.fixed_offset}")
                 return
             record = original_record[column.fixed_offset:]
-            parsed_type = parse_type(column.type, record, version=self.version)
+            parsed_type = parse_type(column.type, record, version=self.version, props=column.extra_props or None)
+            if not has_value:
+                self.parsed_table[column_name].append(None)
+                return
         self.parsed_table[column_name].append(parsed_type)
 
     def _parse_dynamic_length_records_metadata(self, reverse_record, original_record, null_table_length):
         """
         parse the metadata of relative records. The metadata used to parse relative records is found at the end of the
         record so reverse_record is used for parsing from the bottom up.
         :param reverse_record: original record in reverse
@@ -322,26 +379,36 @@
                 logging.warning(
                     f"Record did not parse correctly. Number of columns: {self.table_header.variable_columns}"
                     f" number of parsed columns: {relative_record_metadata.variable_length_field_count}")
                 return None
         return relative_record_metadata
 
     def _parse_dynamic_length_data(self, original_record, relative_record_metadata,
-                                   relative_records_column_map):
+                                   relative_records_column_map, null_table):
         """
         Parse dynamic (non fixed length) records from row
         :param original_record: full unmodified record
         :param relative_record_metadata: parsed record metadata
         :param relative_records_column_map: relative records colum mapping {index: column}
+        :param null_table: list indicating which columns have null value
         """
         relative_offsets = relative_record_metadata.variable_length_field_offsets
         jump_table_addition = 0
         for i, column_index in enumerate(relative_records_column_map):
             column = relative_records_column_map[column_index]
             col_name = column.col_name_str
+            has_value = True
+            if column.column_id > len(null_table):
+                logging.warning("Invalid null table. null values may be shown in the db.")
+            else:
+                has_value = null_table[column.column_id]
+            if not has_value:
+                self.parsed_table[col_name].append(None)
+                continue
+
             if self.version == 3:
                 if i in relative_record_metadata.variable_length_jump_table:
                     jump_table_addition += 0x100
             rel_start = relative_offsets[i]
             # If this is the last one use var_len_count as end offset
             if i + 1 == len(relative_offsets):
                 rel_end = relative_record_metadata.var_len_count
@@ -353,18 +420,24 @@
                 self.parsed_table[col_name].append("")
                 continue
 
             relative_obj_data = original_record[rel_start + jump_table_addition: rel_end + jump_table_addition]
             # Parse types that require column data here, call parse_type on all other types
             if column.type == TYPE_MEMO:
                 try:
-                    parsed_type = self._parse_memo(relative_obj_data, column)
+                    parsed_type = self._parse_memo(relative_obj_data)
                 except ConstructError:
                     logging.warning("Failed to parse memo field. Using data as bytes")
                     parsed_type = relative_obj_data
+            elif column.type == TYPE_OLE:
+                try:
+                    parsed_type = self._parse_memo(relative_obj_data, return_raw=True)
+                except ConstructError:
+                    logging.warning("Failed to parse OLE field. Using data as bytes")
+                    parsed_type = relative_obj_data
             elif column.type == TYPE_96_bit_17_BYTES:
                 if len(relative_obj_data) != 17:
                     logging.warning(f"Relative numeric field has invalid length {len(relative_obj_data)}, expected 17")
                     parsed_type = relative_obj_data
                 else:
                     # Get scale or None
                     scale = column.get('various', {}).get('scale', 6)
@@ -392,29 +465,36 @@
 
         except ConstructError:
             logging.error(f"Failed to parse table header {self.table.value}")
             return
         col_names = table_header.column_names
         columns = table_header.column
 
-        # Add names to columns metadata so we can use only columns for parsing
+        # Add names to columns metadata, so we can use only columns for parsing
         for i, c in enumerate(columns):
             c.col_name_str = col_names[i].col_name_str
+            c.extra_props = None
 
         # column_index is more accurate(id is always incremented so it is wrong when a column is deleted).
         # Some tables like the catalog don't have index, so if indexes are 0 use id.
 
         # create a dict of index to column to make it easier to access. offset is used to make this zero based
         offset = min(x.column_index for x in columns)
         column_dict = {x.column_index - offset: x for x in columns}
         # If column index is not unique try best effort
         if len(column_dict) != len(columns):
             # create a dict of id to column to make it easier to access
             column_dict = {x.column_id: x for x in columns}
 
+        # Add the extra properties relevant for the column
+        if self.props:
+            for i, col in column_dict.items():
+                if col.col_name_str in self.props:
+                    col.extra_props = self.props[col.col_name_str]
+
         if len(column_dict) != table_header.column_count:
             logging.debug(f"expected {table_header.column_count} columns got {len(column_dict)}")
         return column_dict, table_header
 
     def _merge_table_data(self, first_page):
         """
         Merege data of tdef pages in case the data does not fit in one page
@@ -426,36 +506,45 @@
         data = table[parsed_header.header_end:]
         while parsed_header.next_page_ptr:
             table = self._table_defs.get(parsed_header.next_page_ptr * self.page_size)
             parsed_header = TDEF_HEADER.parse(table)
             data = data + table[parsed_header.header_end:]
         return data
 
-    def _parse_memo(self, relative_obj_data, column):
+    def _parse_memo(self, relative_obj_data, return_raw=False):
         logging.debug(f"Parsing memo field {relative_obj_data}")
         parsed_memo = MEMO.parse(relative_obj_data)
+        memo_type = TYPE_TEXT
         if parsed_memo.memo_length & 0x80000000:
             logging.debug("memo data inline")
             inline_memo_length = parsed_memo.memo_length & 0x3FFFFFFF
             if len(relative_obj_data) < parsed_memo.memo_end + inline_memo_length:
                 logging.warning("Inline memo field has invalid length using full data")
                 memo_data = relative_obj_data[parsed_memo.memo_end:]
             else:
                 memo_data = relative_obj_data[parsed_memo.memo_end:parsed_memo.memo_end + inline_memo_length]
-            memo_type = TYPE_TEXT
+
         elif parsed_memo.memo_length & 0x40000000:
             logging.debug("LVAL type 1")
             memo_data = self._get_overflow_record(parsed_memo.record_pointer)
-            memo_type = TYPE_TEXT
         else:
             logging.debug("LVAL type 2")
-            logging.warning("memo lval type 2 currently not supported")
-            memo_data = relative_obj_data
-            memo_type = column.type
+            rec_data = self._get_overflow_record(parsed_memo.record_pointer)
+            next_page = struct.unpack("I", rec_data[:4])[0]
+            # LVAL2 has data over multiple pages. The first 4 bytes of the page are the next record, then that data.
+            # Concat the data until we get a 0 next_page.
+            memo_data = b""
+            while next_page:
+                memo_data += rec_data[4:]
+                rec_data = self._get_overflow_record(next_page)
+                next_page = struct.unpack("I", rec_data[:4])[0]
+            memo_data += rec_data[4:]
         if memo_data:
+            if return_raw:
+                return memo_data
             parsed_type = parse_type(memo_type, memo_data, len(memo_data), version=self.version)
             return parsed_type
 
     def _get_overflow_record(self, record_pointer):
         """
         Get the actual record from a record pointer
         :param record_pointer:
@@ -476,11 +565,11 @@
             start = start & 0xfff
         else:
             logging.debug(f"Overflow record flag is not present {start}")
         if record_offset == 0:
             record = record_page[start:]
         else:
             end = parsed_data.record_offsets[record_offset - 1]
-            if end & 0x8000:
+            if end & 0x8000 and (end & 0xff != 0):
                 end = end & 0xfff
             record = record_page[start: end]
         return record
```

### Comparing `access_parser-0.0.4/access_parser/parsing_primitives.py` & `access_parser-0.0.5/access_parser/parsing_primitives.py`

 * *Files 20% similar despite different names*

```diff
@@ -59,14 +59,55 @@
 TDEF_HEADER = Struct(
     Const(b'\02\x01'),
     "peek_version" / Peek(Int16ul),
     "tdef_ver" / IfThenElse(lambda x: x.peek_version == b"VC", Const(b"VC"), Int16ul),
     "next_page_ptr" / Int32ul,
     "header_end" / Tell)
 
+LVPROP_CHUNK_NAMES_INT = Struct(
+    "name_length" / Int16ul,
+    "name" / PaddedString(this.name_length, "utf16"),
+)
+LVPROP_CHUNK_NAMES = Struct(
+    "names" / GreedyRange(LVPROP_CHUNK_NAMES_INT),
+    # "leftover" / GreedyBytes
+)
+LVPROP_DATA = Struct(
+    "data_length" / Int16ul,
+    "ddl_flag" / Int8ul,
+    "type" / Int8ul,
+    "name_index" / Int16ul,
+    "only_data_length" / Int16ul,
+    "actual_data" / Bytes(this.only_data_length)
+)
+LVPROP_VALUE = Struct(
+    "val_length" / Int32ul,
+    "name_length" / Int16ul,
+    "column_name" / PaddedString(this.name_length, "utf16"),
+    "data" / GreedyRange(LVPROP_DATA),
+    "left" / GreedyBytes
+)
+
+LVPROP_CHUNK = Struct(
+    "length" / Int32ul,
+    "chunk_type" / Int16ul,
+
+    "data" / Prefixed(Computed(this.length - 6), Switch(this.chunk_type, {
+        # 128: GreedyRange(LVPROP_CHUNK_NAMES)
+        128: LVPROP_CHUNK_NAMES,
+        0:LVPROP_VALUE,
+        1: LVPROP_VALUE
+    }, default=Bytes(this.length - 4)))
+)
+LVPROP = Struct(
+    #'KKD\0' in Jet3 and 'MR2\0' in Jet 4.
+    "magic" / Bytes(4),
+    "chunks" / GreedyRange(LVPROP_CHUNK),
+    "leftover" / GreedyBytes
+)
 
 def parse_table_head(buffer, version=3):
     REAL_INDEX2 = Struct(
         "unknown_b1" / If(lambda x: version > 3, Int32ul),
         "unk_struct" / Array(10, Struct("col_id" / Int16ul, "idx_flags" / Int8ul)),
         "runk" / Int32ul,
         "first_index_page" / Int32ul,
```

### Comparing `access_parser-0.0.4/access_parser.egg-info/PKG-INFO` & `access_parser-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,59 @@
 Metadata-Version: 2.1
-Name: access-parser
-Version: 0.0.4
+Name: access_parser
+Version: 0.0.5
 Summary: Access database (*.mdb, *.accdb) parser
 Home-page: https://github.com/ClarotyICS/access_parser
 Author: Uri Katz
 Author-email: uri.k@claroty.com
-License: UNKNOWN
-Description: # AccessDB Parser
-        Microsoft Access (.mdb / .accdb) database files parser. The parsing logic is fully written in python and works without any external binary dependencies.
-        
-        # Installing
-        Use pip: `pip install access-parser`
-        
-        Or install manually:
-        ```bash
-        git clone https://github.com/ClarotyICS/access_parser.git
-        cd access_parser
-        python3 setup.py install
-        ```
-        
-        # Demo
-        [![asciicast](https://asciinema.org/a/345445.svg)](https://asciinema.org/a/345445)
-        
-        # Usage Example
-        ```python
-        from access_parser import AccessParser
-        
-        # .mdb or .accdb file
-        db = AccessParser("/path/to/mdb/file.mdb")
-        
-        # Print DB tables
-        print(db.catalog)
-        
-        # Tables are stored as defaultdict(list) -- table[column][row_index]
-        table = db.parse_table("table_name")
-        
-        # Pretty print all tables
-        db.print_database()
-        
-        ```
-        
-        ### Known Issues
-        * OLE fields are currently not supported
-        * Only a subset of memo fields are parsed
-        
-        This library was tested on a limited subset of database files. Due to the differences between database versions and the complexity of the parsing we expect to find more parsing edge-cases.
-        
-        To help us resolve issues faster please provide as much data as you can when opening an issue - DB file if possible and full trace including log messages.
-         
-         
-        ### Thanks
-        * This library was made possible by the great work by mdb-tools. The logic in this library heavily relies on the excellent documentation they have https://github.com/brianb/mdbtools
-        * Huge thanks to Mashav Sapir for the help debugging, CRing and contributing to this project https://github.com/mashavs
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AccessDB Parser (Pure Python)
+Microsoft Access (.mdb / .accdb) database files parser. The parsing logic is fully written in python and works without any external binary dependencies.
+
+# Installing
+Use pip: `pip install access-parser`
+
+Or install manually:
+```bash
+git clone https://github.com/ClarotyICS/access_parser.git
+cd access_parser
+python3 setup.py install
+```
+
+# Demo
+[![asciicast](https://asciinema.org/a/345445.svg)](https://asciinema.org/a/345445)
+
+# Usage Example
+```python
+from access_parser import AccessParser
+
+# .mdb or .accdb file
+db = AccessParser("/path/to/mdb/file.mdb")
+
+# Print DB tables
+print(db.catalog)
+
+# Tables are stored as defaultdict(list) -- table[column][row_index]
+table = db.parse_table("table_name")
+
+# Pretty print all tables
+db.print_database()
+
+```
+
+### Known Issues
+* 
+
+This library was tested on a limited subset of database files. Due to the differences between database versions and the complexity of the parsing we expect to find more parsing edge-cases.
+
+To help us resolve issues faster please provide as much data as you can when opening an issue - DB file if possible and full trace including log messages.
+ 
+ 
+### Thanks
+* This library was made possible by the great work by mdb-tools. The logic in this library heavily relies on the excellent documentation they have https://github.com/brianb/mdbtools
+* Huge thanks to Mashav Sapir for the help debugging, CRing and contributing to this project https://github.com/mashavs
```

### Comparing `access_parser-0.0.4/README.md` & `access_parser-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AccessDB Parser
+# AccessDB Parser (Pure Python)
 Microsoft Access (.mdb / .accdb) database files parser. The parsing logic is fully written in python and works without any external binary dependencies.
 
 # Installing
 Use pip: `pip install access-parser`
 
 Or install manually:
 ```bash
@@ -29,16 +29,15 @@
 
 # Pretty print all tables
 db.print_database()
 
 ```
 
 ### Known Issues
-* OLE fields are currently not supported
-* Only a subset of memo fields are parsed
+* 
 
 This library was tested on a limited subset of database files. Due to the differences between database versions and the complexity of the parsing we expect to find more parsing edge-cases.
 
 To help us resolve issues faster please provide as much data as you can when opening an issue - DB file if possible and full trace including log messages.
  
  
 ### Thanks
```

### Comparing `access_parser-0.0.4/setup.py` & `access_parser-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="access_parser",
-    version="0.0.4",
+    version="0.0.5",
     author="Uri Katz",
     author_email="uri.k@claroty.com",
     description="Access database (*.mdb, *.accdb) parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ClarotyICS/access_parser",
     packages=setuptools.find_packages(),
```

