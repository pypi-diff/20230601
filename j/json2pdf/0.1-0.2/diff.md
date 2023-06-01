# Comparing `tmp/json2pdf-0.1.tar.gz` & `tmp/json2pdf-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json2pdf-0.1.tar", last modified: Thu Jun  1 19:53:08 2023, max compression
+gzip compressed data, was "json2pdf-0.2.tar", last modified: Thu Jun  1 19:59:15 2023, max compression
```

## Comparing `json2pdf-0.1.tar` & `json2pdf-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:53:08.621672 json2pdf-0.1/
--rw-rw-rw-   0        0        0     2266 2023-06-01 19:53:08.620256 json2pdf-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2168 2023-06-01 19:37:58.000000 json2pdf-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:53:08.619251 json2pdf-0.1/json2pdf.egg-info/
--rw-rw-rw-   0        0        0     2266 2023-06-01 19:53:08.000000 json2pdf-0.1/json2pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-06-01 19:53:08.000000 json2pdf-0.1/json2pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:53:08.000000 json2pdf-0.1/json2pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-01 19:53:08.000000 json2pdf-0.1/json2pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 19:53:08.000000 json2pdf-0.1/json2pdf.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 19:53:08.620256 json2pdf-0.1/pdf_generator/
--rw-rw-rw-   0        0        0     5640 2023-06-01 19:32:12.000000 json2pdf-0.1/pdf_generator/convert.py
--rw-rw-rw-   0        0        0      231 2023-06-01 19:50:41.000000 json2pdf-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 19:53:08.621672 json2pdf-0.1/setup.cfg
--rw-rw-rw-   0        0        0      423 2023-06-01 19:42:49.000000 json2pdf-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:15.057771 json2pdf-0.2/
+-rw-rw-rw-   0        0        0     2266 2023-06-01 19:59:15.033336 json2pdf-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-06-01 19:37:58.000000 json2pdf-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:15.029961 json2pdf-0.2/json2pdf.egg-info/
+-rw-rw-rw-   0        0        0     2266 2023-06-01 19:59:14.000000 json2pdf-0.2/json2pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-06-01 19:59:14.000000 json2pdf-0.2/json2pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:59:14.000000 json2pdf-0.2/json2pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-01 19:59:14.000000 json2pdf-0.2/json2pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 19:59:14.000000 json2pdf-0.2/json2pdf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:59:15.032007 json2pdf-0.2/pdf_generator/
+-rw-rw-rw-   0        0        0     5663 2023-06-01 19:57:18.000000 json2pdf-0.2/pdf_generator/convert.py
+-rw-rw-rw-   0        0        0      231 2023-06-01 19:57:40.000000 json2pdf-0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:59:15.057771 json2pdf-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-06-01 19:42:49.000000 json2pdf-0.2/setup.py
```

### Comparing `json2pdf-0.1/PKG-INFO` & `json2pdf-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json2pdf
-Version: 0.1
+Version: 0.2
 Description-Content-Type: text/markdown
 
 To create the content for the README.md file of your Python package, you can include the following information:
 
 # PDF Generator
 
 A Python package for converting JSON data to HTML and generating PDFs.
```

### Comparing `json2pdf-0.1/README.md` & `json2pdf-0.2/README.md`

 * *Files identical despite different names*

### Comparing `json2pdf-0.1/json2pdf.egg-info/PKG-INFO` & `json2pdf-0.2/json2pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json2pdf
-Version: 0.1
+Version: 0.2
 Description-Content-Type: text/markdown
 
 To create the content for the README.md file of your Python package, you can include the following information:
 
 # PDF Generator
 
 A Python package for converting JSON data to HTML and generating PDFs.
```

### Comparing `json2pdf-0.1/pdf_generator/convert.py` & `json2pdf-0.2/pdf_generator/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     with open(output_html_path, 'w', encoding='utf-8') as file:
         file.write(html_content)
     print(f'HTML file created: {output_html_path}')
 
     # Rest of the code...
     start_time = time.time()
-    print(start_time)
+    print("PDF Creation Started")
 
     # Calculate the total number of lines in the HTML content
     total_lines = len(html_content.split('\n'))
     print(f'Total lines: {total_lines}')
 
     # Define the number of lines per chunk
     lines_per_chunk = total_lines  # Adjust this value as per your requirement
@@ -141,14 +141,14 @@
     merged_pdf_file = os.path.join(output_pdf_directory, 'merged_output.pdf')
 
     merger.write(merged_pdf_file)
     merger.close()
     elapsed_time = time.time() - start_time
 
     print(f'PDF file created: {merged_pdf_file}')
-    print(f'Elapsed time: {elapsed_time / 60} minutes')
+    print(f'PDF created in time: {elapsed_time / 60:.2f} minutes')
 
     # Delete the individual PDF files (optional)
     for pdf_file in pdf_files:
         os.remove(pdf_file)
```

