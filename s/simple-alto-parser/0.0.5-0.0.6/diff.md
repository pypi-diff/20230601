# Comparing `tmp/simple-alto-parser-0.0.5.tar.gz` & `tmp/simple-alto-parser-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-alto-parser-0.0.5.tar", last modified: Wed May 24 14:10:37 2023, max compression
+gzip compressed data, was "simple-alto-parser-0.0.6.tar", last modified: Thu Jun  1 12:43:53 2023, max compression
```

## Comparing `simple-alto-parser-0.0.5.tar` & `simple-alto-parser-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/simple_alto_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/alto_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/dictionary_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/dictionary_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/nlp_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-24 14:10:23.000000 simple-alto-parser-0.0.5/simple_alto_parser/pattern_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:10:37.382781 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 14:10:37.000000 simple-alto-parser-0.0.5/simple_alto_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/simple_alto_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/dictionary_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/dictionary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/nlp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/pattern_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/top_level.txt
```

### Comparing `simple-alto-parser-0.0.5/LICENSE` & `simple-alto-parser-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.5/PKG-INFO` & `simple-alto-parser-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -21,17 +21,9 @@
 # simple-alto-parser
 This is a simple parser for ALTO XML files. It is designed to do two tasks separately:
 1. Extract the text from the ALTO XML file with the AltoTextParser class.
 2. Extract structured information from the text with different parsing methods.
 
 ## Usage
 ```python
-from simple_alto_parser import AltoTextParser
 
-alto_parser = AltoTextParser()
-alto_parser.add_file('path/to/alto.xml')
-alto_parser.parse_text()
-
-result = alto_parser.get_alto_files()
-regions = result[0].get_text_regions()
-lines = regions[0].get_text_lines()
 ```
```

### Comparing `simple-alto-parser-0.0.5/setup.cfg` & `simple-alto-parser-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/alto_file.py` & `simple-alto-parser-0.0.6/simple_alto_parser/alto_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,18 @@
             raise ValueError("The given path is not a file.")
 
         self.file_path = file_path
         self.file_meta_data = {}
         self.parser = parser
         self.file_elements = []
 
+    def has_lines(self):
+        """This function returns True if the file has lines, otherwise it returns False."""
+        return len(self.file_elements) > 0
+
     def get_text_lines(self):
         """This function returns the text lines of the alto file."""
         return self.file_elements
 
     def add_file_meta_data(self, parameter_name, parameter_value):
         """This function adds metadata to the file. It takes the parameter name and the parameter value as parameters.
         The parameter name should be a string and the parameter value can be any type."""
@@ -43,80 +47,85 @@
         for file_element in self.file_elements:
             for key, value in file_element.parser_data.items():
                 parser_keys.append(key)
         parser_keys = list(set(parser_keys))
         return parser_keys
 
     def get_csv_header(self):
-        """This function returns the header of a single csv file. It is used by the export_to_csv() function."""
-
-        print_manipulated = self.parser.get_config_value('export', 'csv', 'print_manipulated', default=False)
-        print_filename = self.parser.get_config_value('export', 'csv', 'print_filename', default=False)
-        print_attributes = self.parser.get_config_value('export', 'csv', 'print_attributes', default=False)
-        print_parser_results = self.parser.get_config_value('export', 'csv', 'print_parser_results', default=False)
-        print_file_meta_data = self.parser.get_config_value('export', 'csv', 'print_file_meta_data', default=False)
-
-        csv_title_line = ['original_text']
-        if print_manipulated:
-            csv_title_line.append('manipulated_text')
-        if print_filename:
-            csv_title_line.append('file')
-        if print_attributes:
-            for key, value in self.file_elements[0].element_data.items():
-                csv_title_line.append(key)
-        if print_parser_results:
-            # Create a list of all parser keys
-            csv_title_line += self.get_parser_result_keys()
-
-        if print_file_meta_data:
-            for key, value in self.file_meta_data.items():
-                csv_title_line.append(key)
-
-        return csv_title_line
-
-    def get_csv_lines(self, add_header=True):
-
-        header = self.get_csv_header()
-        if add_header:
-            csv_lines = [header, ]
-        else:
-            csv_lines = []
-
-        lines = self.get_text_lines()
+        if self.has_lines():
+            """This function returns the header of a single csv file. It is used by the export_to_csv() function."""
 
-        if len(lines) == 0:
-            raise ValueError("No lines have been found in the file.")
+            print_manipulated = self.parser.get_config_value('export', 'csv', 'print_manipulated', default=False)
+            print_filename = self.parser.get_config_value('export', 'csv', 'print_filename', default=False)
+            print_attributes = self.parser.get_config_value('export', 'csv', 'print_attributes', default=False)
+            print_parser_results = self.parser.get_config_value('export', 'csv', 'print_parser_results', default=False)
+            print_file_meta_data = self.parser.get_config_value('export', 'csv', 'print_file_meta_data', default=False)
 
-        print_manipulated = self.parser.get_config_value('export', 'csv', 'print_manipulated', default=False)
-        print_attributes = self.parser.get_config_value('export', 'csv', 'print_attributes', default=False)
-        print_parser_results = self.parser.get_config_value('export', 'csv', 'print_parser_results', default=False)
-        print_filename = self.parser.get_config_value('export', 'csv', 'print_filename', default=False)
-        print_file_meta_data = self.parser.get_config_value('export', 'csv', 'print_file_meta_data', default=False)
-
-        for line in lines:
-            csv_line = [line.get_original_text()]
+            csv_title_line = ['original_text']
             if print_manipulated:
-                csv_line.append(line.get_text())
+                csv_title_line.append('manipulated_text')
             if print_filename:
-                csv_line.append(self.file_path)
-
+                csv_title_line.append('file')
             if print_attributes:
-                for key, value in line.element_data.items():
-                    csv_line.append(value)
-
+                for key, value in self.file_elements[0].element_data.items():
+                    csv_title_line.append(key)
             if print_parser_results:
-                for parser_val in self.get_parser_result_keys():
-                    csv_line.append(line.parser_data.get(parser_val, ''))
+                # Create a list of all parser keys
+                csv_title_line += self.get_parser_result_keys()
 
             if print_file_meta_data:
                 for key, value in self.file_meta_data.items():
-                    csv_line.append(value)
-            csv_lines.append(csv_line)
+                    csv_title_line.append(key)
 
-        return csv_lines
+            return csv_title_line
+        else:
+            return []
+
+    def get_csv_lines(self, add_header=True):
+        if self.has_lines():
+            header = self.get_csv_header()
+            if add_header:
+                csv_lines = [header, ]
+            else:
+                csv_lines = []
+
+            lines = self.get_text_lines()
+
+            if len(lines) == 0:
+                raise ValueError("No lines have been found in the file.")
+
+            print_manipulated = self.parser.get_config_value('export', 'csv', 'print_manipulated', default=False)
+            print_attributes = self.parser.get_config_value('export', 'csv', 'print_attributes', default=False)
+            print_parser_results = self.parser.get_config_value('export', 'csv', 'print_parser_results', default=False)
+            print_filename = self.parser.get_config_value('export', 'csv', 'print_filename', default=False)
+            print_file_meta_data = self.parser.get_config_value('export', 'csv', 'print_file_meta_data', default=False)
+
+            for line in lines:
+                csv_line = [line.get_original_text()]
+                if print_manipulated:
+                    csv_line.append(line.get_text())
+                if print_filename:
+                    csv_line.append(self.file_path)
+
+                if print_attributes:
+                    for key, value in line.element_data.items():
+                        csv_line.append(value)
+
+                if print_parser_results:
+                    for parser_val in self.get_parser_result_keys():
+                        csv_line.append(line.parser_data.get(parser_val, ''))
+
+                if print_file_meta_data:
+                    for key, value in self.file_meta_data.items():
+                        csv_line.append(value)
+                csv_lines.append(csv_line)
+
+            return csv_lines
+        else:
+            return []
 
     def get_json_objects(self):
         lines = self.get_text_lines()
 
         json_objects = []
         for line in lines:
             d_line = line.to_dict()
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/alto_file_exporter.py` & `simple-alto-parser-0.0.6/simple_alto_parser/alto_file_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,20 @@
 
         self.save_to_csv(file_name, csv_lines, **kwargs)
 
     def save_csvs(self, directory_name, **kwargs):
         self.assure_is_dir(directory_name)
 
         for file in self.files:
-            csv_lines = file.get_csv_lines(add_header=True)
-            file_name = os.path.join(directory_name, file.get_file_name(ftype='csv'))
-            self.save_to_csv(file_name, csv_lines, **kwargs)
+            if file.has_lines():
+                csv_lines = file.get_csv_lines(add_header=True)
+                file_name = os.path.join(directory_name, file.get_file_name(ftype='csv'))
+                self.save_to_csv(file_name, csv_lines, **kwargs)
+            else:
+                pass
 
     def save_json(self, file_name):
         self.assure_is_file(file_name)
 
         json_objects = []
         for file in self.files:
             json_objects.extend(file.get_json_objects())
@@ -50,19 +53,22 @@
         with open(file_name, 'w', encoding='utf-8') as outfile:
             json.dump(json_objects, outfile, indent=4, sort_keys=True)
 
     def save_jsons(self, directory_name):
         self.assure_is_dir(directory_name)
 
         for file in self.files:
-            json_objects = file.get_json_objects()
-            file_name = os.path.join(directory_name, file.get_file_name(ftype='json'))
-
-            with open(file_name, 'w', encoding='utf-8') as f:
-                json.dump(json_objects, f, indent=4, sort_keys=True)
+            if file.has_lines():
+                json_objects = file.get_json_objects()
+                file_name = os.path.join(directory_name, file.get_file_name(ftype='json'))
+
+                with open(file_name, 'w', encoding='utf-8') as f:
+                    json.dump(json_objects, f, indent=4, sort_keys=True)
+            else:
+                pass
 
     @staticmethod
     def assure_is_file(file_path):
         """Assure that the given path is a file."""
         if not os.path.exists(file_path):
             os.makedirs(os.path.dirname(file_path), exist_ok=True)
             return
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/alto_file_parser.py` & `simple-alto-parser-0.0.6/simple_alto_parser/alto_file_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 """This module contains the class AltoTextParser, which is used to parse text from ALTO files."""
 import os
 import re
+import sys
 import xml.etree.ElementTree as ETree
 from simple_alto_parser.alto_file import AltoFile, AltoFileElement
+from simple_alto_parser.utils import get_logger
 
 
 class AltoFileParser:
     """This class is used to parse text from ALTO files. It stores the files in a list of AltoFile objects."""
 
+    logger = None
+    """The logger of the class."""
+
     LINE_TYPES = ['TextLine', 'TextBlock']
 
     attributes_to_get = ["id", "baseline", "hpos", "vpos", "width", "height"]
     """A list of the attributes that should be stored in the element_data dictionary."""
 
     files = []
 
     def __init__(self, directory_path=None, parser_config=None):
         """The constructor of the class."""
+
+        self.logger = get_logger()
+
         self.parser_config = {
             'line_type': 'TextLine',
             'file_ending': '.xml',
             'export': {                            # Options for exporting the parsed data.
                 'csv': {
                     'print_manipulated': False,      # Print the manipulated text to the csv.
                     'print_filename': False,         # Print the filename to the csv.
@@ -30,14 +38,16 @@
                 }
             }
         }
 
         if parser_config:
             self.parser_config.update(parser_config)
 
+        self.logger.debug("Parser config: %s", self.parser_config)
+
         if directory_path:
             self.add_files(directory_path, self.get_config_value('file_ending'))
         else:
             self.files = []
 
         if 'meta_data' in self.parser_config:
             for key, value in self.parser_config['meta_data'].items():
@@ -50,37 +60,42 @@
 
                 if match and len(match.groups()) == len(self.parser_config['file_name_structure']['value_names']):
                     idx = 1
                     for value_name in self.parser_config['file_name_structure']['value_names']:
                         file.add_file_meta_data(value_name, match.group(idx))
                         idx += 1
                 else:
-                    raise ValueError("The file name structure does not match the given pattern.")
+                    self.logger.warning("The file name structure does not match the file name of the file '%s'.",
+                                        file.file_path)
 
     def add_files(self, directory_path, file_ending='.xml'):
         """Add all files with the given file ending in the given directory to the list of files to be parsed."""
 
         if not os.path.isdir(directory_path):
-            raise ValueError("The given path is not a directory.")
+            self.logger.error("The given path is not a directory.")
+            sys.exit()
 
         for file in os.listdir(directory_path):
             if file.endswith(file_ending):
                 self.add_file(os.path.join(directory_path, file))
+        self.logger.info("Added %s files to the list of files to be parsed.", len(self.files))
 
     def add_file(self, file_path):
         """Add the given file to the list of files to be parsed."""
 
         alto_file = AltoFile(file_path, self)
         self.files.append(alto_file)
+        self.logger.debug("Added file '%s' to the list of files to be parsed.", file_path)
 
     def parse(self):
         """Parse the text from all files in the list of files."""
 
         for alto_file in self.files:
             self.parse_file(alto_file)
+        self.logger.info(f"Parsed text from {len(self.files)} files.")
 
     def parse_file(self, alto_file):
         """This function parses the alto file and stores the data in the class."""
 
         xml_tree, xmlns = self._xml_parse_file(alto_file.file_path)
         if xml_tree is None:
             raise ValueError("The given file is not a valid xml file.")
@@ -122,34 +137,37 @@
         if 'http://' in str(xml_tree.getroot().tag.split('}')[0].strip('{')):
             xmlns = xml_tree.getroot().tag.split('}')[0].strip('{')
         else:
             try:
                 ns = xml_tree.getroot().attrib
                 xmlns = str(ns).split(' ')[1].strip('}').strip("'")
             except IndexError as error:
-                raise error
+                xmlns = ''
+                self.logger.error(f"The given file '{file_path}' is not a valid alto file. {error}")
+                sys.exit()
 
         if xmlns not in namespace.values():
-            raise IndexError('No valid namespace has been found.')
+            self.logger.error(f"The given file '{file_path}' is not a valid alto file.")
+            sys.exit()
 
         return xml_tree, xmlns
 
     def get_alto_files(self):
         """Return the list of AltoFile objects."""
-
         return self.files
 
     def get_attributes(self, element):
         """This function reads the attributes of the element and stores them in the element_data dictionary."""
         attrs = {}
         for attribute in self.attributes_to_get:
             try:
                 attrs[attribute] = element.attrib.get(attribute.upper())
             except KeyError:
                 # The attribute is not in the element. This is not a problem.
+                self.logger.debug(f"The attribute '%s' is not in the element.", attribute)
                 pass
         return attrs
 
     @staticmethod
     def sanitize_text(text):
         """This function removes all line breaks, tabs and carriage returns from the text and removes leading and
         trailing whitespaces."""
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/base_parser.py` & `simple-alto-parser-0.0.6/simple_alto_parser/base_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from simple_alto_parser.utils import get_logger
+
+
 class BaseParser:
 
+    logger = None
     matches = []
 
     def __init__(self, parser):
         """The constructor of the class. It initializes the list of files.
         The lines are a list of AltoXMLElement objects."""
+        self.logger = get_logger()
         self.parser = parser
         self.matches = []
 
     def mark(self, name, value):
         """Add the given category to all matches."""
         for match in self.matches:
             self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].add_parser_data(name, value)
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/dictionary_creator.py` & `simple-alto-parser-0.0.6/simple_alto_parser/dictionary_creator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 import csv
 import json
 
+class AltoDictionaryCreator:
 
-def from_geonames(csv_file_path):
-    # Open Tsv
-    with open(csv_file_path, encoding='utf-8') as f:
-        csv_reader = csv.reader(f, delimiter='\t')
-        row_id = 0
-        for row in csv_reader:
-            if row[6] == 'P':
-                print(
-                    row[0],  # geonames_id
-                    row[1],  # name
-                    row[2],  # asciiname
-                    row[3],  # alternatenames
-                    row[4],  # latitude
-                    row[5],  # longitude
-                    row[6],  # feature_class
-                    row[7],  # feature_code
-                    row[8],  # country_code
-                    row[9],  # cc2
-                    row[10],  # admin1_code
-                    row[11],  # admin2_code
-                    row[12],  # admin3_code
-                    row[13],  # admin4_code
-                    row[14],  # population
-                    row[15],  # elevation
-                    row[16],  # dem
-                    row[17],  # timezone
-                    row[18]  # modification_date
-                )
-
-
-            row_id += 1
-            if row_id > 20:
-                break
-
-
-#from_geonames('../assets/dicts/CH.tsv')
-
-def from_file(filename, type='undefined'):
-    with open(filename, encoding='utf-8') as f:
-        entries = []
-        for line in f:
-            entry = {
-                "label": line.strip(),
-                "variants": [line.strip()],
-                "type": type
-            }
-            entries.append(entry)
+    @staticmethod
+    def from_file(input_filename, output_filename, type='undefined'):
+        with open(input_filename, encoding='utf-8') as f:
+            entries = []
+            for line in f:
+                entry = {
+                    "label": line.strip(),
+                    "variants": [line.strip()],
+                    "type": type
+                }
+                entries.append(entry)
+
+        with open(output_filename, 'w', encoding='utf-8') as f:
+            f.write(json.dumps(entries, indent=4, sort_keys=True))
+
+    def from_geonames(self, csv_file_path):
+        # Open Tsv
+        with open(csv_file_path, encoding='utf-8') as f:
+            csv_reader = csv.reader(f, delimiter='\t')
+            row_id = 0
+            for row in csv_reader:
+                if row[6] == 'P':
+                    print(
+                        row[0],  # geonames_id
+                        row[1],  # name
+                        row[2],  # asciiname
+                        row[3],  # alternatenames
+                        row[4],  # latitude
+                        row[5],  # longitude
+                        row[6],  # feature_class
+                        row[7],  # feature_code
+                        row[8],  # country_code
+                        row[9],  # cc2
+                        row[10],  # admin1_code
+                        row[11],  # admin2_code
+                        row[12],  # admin3_code
+                        row[13],  # admin4_code
+                        row[14],  # population
+                        row[15],  # elevation
+                        row[16],  # dem
+                        row[17],  # timezone
+                        row[18]  # modification_date
+                    )
+
+
+                row_id += 1
+                if row_id > 20:
+                    break
 
-    with open(filename + '.json', 'w', encoding='utf-8') as f:
-        f.write(json.dumps(entries, indent=4, sort_keys=True))
-
-from_file('../assets/dicts/titles.csv', type="title")
+# from_file('../assets/dicts/titles.csv', type="title")
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/dictionary_parser.py` & `simple-alto-parser-0.0.6/simple_alto_parser/dictionary_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 import json
 import re
+import sys
 
 from simple_alto_parser import BaseParser
 from simple_alto_parser.base_parser import ParserMatch
 
 
 class AltoDictionaryParser(BaseParser):
+    """This class is used to find patterns in the text lines of an alto file."""
 
     dictionaries = []
 
     def __init__(self, parser):
         """The constructor of the class. It initializes the list of files.
         The lines are a list of AltoXMLElement objects."""
         super().__init__(parser)
 
     def load(self, dictionary_file):
+        self.logger.debug(f"PROBLEM: {dictionary_file}")
+        print("LOAD", dictionary_file)
+
         dictionary = json.load(open(dictionary_file, encoding='utf-8'))
         for entry in dictionary:
             if 'label' in entry:
                 if 'variants' not in entry:
                     entry['variants'] = [entry['label']]
                 if 'type' not in entry:
                     entry['type'] = 'undefined'
 
                 entry['variants'] = [v.strip() for v in entry['variants']]
                 entry['variants'] = sorted(entry['variants'], key=len, reverse=True)
-                print(entry['variants'])
             else:
-                raise Exception('The dictionary entry does not contain a label.')
+                self.logger.error(f'Dictionary Entry "{entry}" from dictionary "{dictionary_file}" has no label.')
+                sys.exit()
 
         self.dictionaries.append(dictionary)
+        self.logger.debug(f"Loaded dictionary: {dictionary_file}")
 
     def find(self, strict=True, restrict_to=None):
         """Find a pattern in the text lines."""
         self.clear()
         file_id = 0
         for file in self.parser.get_alto_files():
             line_id = 0
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/nlp_parser.py` & `simple-alto-parser-0.0.6/simple_alto_parser/nlp_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser/pattern_parser.py` & `simple-alto-parser-0.0.6/simple_alto_parser/pattern_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser.egg-info/PKG-INFO` & `simple-alto-parser-0.0.6/simple_alto_parser.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
@@ -21,17 +21,9 @@
 # simple-alto-parser
 This is a simple parser for ALTO XML files. It is designed to do two tasks separately:
 1. Extract the text from the ALTO XML file with the AltoTextParser class.
 2. Extract structured information from the text with different parsing methods.
 
 ## Usage
 ```python
-from simple_alto_parser import AltoTextParser
 
-alto_parser = AltoTextParser()
-alto_parser.add_file('path/to/alto.xml')
-alto_parser.parse_text()
-
-result = alto_parser.get_alto_files()
-regions = result[0].get_text_regions()
-lines = regions[0].get_text_lines()
 ```
```

### Comparing `simple-alto-parser-0.0.5/simple_alto_parser.egg-info/SOURCES.txt` & `simple-alto-parser-0.0.6/simple_alto_parser.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 simple_alto_parser/alto_file_exporter.py
 simple_alto_parser/alto_file_parser.py
 simple_alto_parser/base_parser.py
 simple_alto_parser/dictionary_creator.py
 simple_alto_parser/dictionary_parser.py
 simple_alto_parser/nlp_parser.py
 simple_alto_parser/pattern_parser.py
+simple_alto_parser/utils.py
 simple_alto_parser.egg-info/PKG-INFO
 simple_alto_parser.egg-info/SOURCES.txt
 simple_alto_parser.egg-info/dependency_links.txt
 simple_alto_parser.egg-info/requires.txt
 simple_alto_parser.egg-info/top_level.txt
```

