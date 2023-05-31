# Comparing `tmp/oneoneoneexample-0.3.tar.gz` & `tmp/oneoneoneexample-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneoneoneexample-0.3.tar", last modified: Wed May 31 22:03:12 2023, max compression
+gzip compressed data, was "oneoneoneexample-0.4.tar", last modified: Wed May 31 22:16:29 2023, max compression
```

## Comparing `oneoneoneexample-0.3.tar` & `oneoneoneexample-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:12.499021 oneoneoneexample-0.3/
--rw-rw-rw-   0        0        0       61 2023-05-31 22:03:12.496330 oneoneoneexample-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-31 18:11:11.000000 oneoneoneexample-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:12.432390 oneoneoneexample-0.3/oneoneoneexample.egg-info/
--rw-rw-rw-   0        0        0       61 2023-05-31 22:03:12.000000 oneoneoneexample-0.3/oneoneoneexample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-05-31 22:03:12.000000 oneoneoneexample-0.3/oneoneoneexample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:03:12.000000 oneoneoneexample-0.3/oneoneoneexample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-31 22:03:12.000000 oneoneoneexample-0.3/oneoneoneexample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 22:03:12.000000 oneoneoneexample-0.3/oneoneoneexample.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 22:03:12.456553 oneoneoneexample-0.3/pdf_generator/
--rw-rw-rw-   0        0        0     4940 2023-05-31 22:00:35.000000 oneoneoneexample-0.3/pdf_generator/convert.py
--rw-rw-rw-   0        0        0      239 2023-05-31 22:00:56.000000 oneoneoneexample-0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 22:03:12.499021 oneoneoneexample-0.3/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/
+-rw-rw-rw-   0        0        0       61 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-31 18:11:11.000000 oneoneoneexample-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.351924 oneoneoneexample-0.4/oneoneoneexample.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 22:16:29.000000 oneoneoneexample-0.4/oneoneoneexample.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 22:16:29.364038 oneoneoneexample-0.4/pdf_generator/
+-rw-rw-rw-   0        0        0     4934 2023-05-31 22:14:27.000000 oneoneoneexample-0.4/pdf_generator/convert.py
+-rw-rw-rw-   0        0        0      239 2023-05-31 22:14:47.000000 oneoneoneexample-0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:16:29.369442 oneoneoneexample-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.4/setup.py
```

### Comparing `oneoneoneexample-0.3/pdf_generator/convert.py` & `oneoneoneexample-0.4/pdf_generator/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,18 +58,16 @@
     # Convert JSON to DataFrame
     df = pd.read_json(json_text)
 
     # Convert DataFrame to list of dictionaries
     data = df.to_dict(orient='records')
 
     # Load HTML template using Jinja2
-    merged_pdf_file = path_to_template
-    print(merged_pdf_file)
     env = Environment(loader=FileSystemLoader('.'))
-    template = env.get_template(merged_pdf_file)
+    template = env.get_template(path_to_template)
 
     # Render HTML from the template with dynamic data
     html_content = template.render(data=data)
 
     html_file = 'output.html'
     with open(html_file, 'w', encoding='utf-8') as file:
         file.write(html_content)
@@ -133,7 +131,8 @@
     print(f'PDF file created: {path_for_merged_pdf}')
     print(f'Elapsed time: {elapsed_time / 60} minutes')
 
     # Delete the individual PDF files (optional)
     for pdf_file in pdf_files:
         os.remove(pdf_file)
 
+generate(path_to_json, path_to_template, path_for_merged_pdf)
```

