# Comparing `tmp/oneoneoneexample-0.6.tar.gz` & `tmp/oneoneoneexample-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oneoneoneexample-0.6.tar", last modified: Thu Jun  1 19:25:35 2023, max compression
+gzip compressed data, was "oneoneoneexample-0.7.tar", last modified: Thu Jun  1 19:39:49 2023, max compression
```

## Comparing `oneoneoneexample-0.6.tar` & `oneoneoneexample-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:25:35.725190 oneoneoneexample-0.6/
--rw-rw-rw-   0        0        0       61 2023-06-01 19:25:35.724156 oneoneoneexample-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-31 18:11:11.000000 oneoneoneexample-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 19:25:35.711004 oneoneoneexample-0.6/oneoneoneexample.egg-info/
--rw-rw-rw-   0        0        0       61 2023-06-01 19:25:35.000000 oneoneoneexample-0.6/oneoneoneexample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-01 19:25:35.000000 oneoneoneexample-0.6/oneoneoneexample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 19:25:35.000000 oneoneoneexample-0.6/oneoneoneexample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-01 19:25:35.000000 oneoneoneexample-0.6/oneoneoneexample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 19:25:35.000000 oneoneoneexample-0.6/oneoneoneexample.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 19:25:35.712530 oneoneoneexample-0.6/pdf_generator/
--rw-rw-rw-   0        0        0     5857 2023-06-01 19:21:43.000000 oneoneoneexample-0.6/pdf_generator/convert.py
--rw-rw-rw-   0        0        0      239 2023-06-01 19:23:55.000000 oneoneoneexample-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 19:25:35.725190 oneoneoneexample-0.6/setup.cfg
--rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.500258 oneoneoneexample-0.7/
+-rw-rw-rw-   0        0        0       61 2023-06-01 19:39:49.499178 oneoneoneexample-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2168 2023-06-01 19:37:58.000000 oneoneoneexample-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.476494 oneoneoneexample-0.7/oneoneoneexample.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 19:39:49.000000 oneoneoneexample-0.7/oneoneoneexample.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 19:39:49.487291 oneoneoneexample-0.7/pdf_generator/
+-rw-rw-rw-   0        0        0     5640 2023-06-01 19:32:12.000000 oneoneoneexample-0.7/pdf_generator/convert.py
+-rw-rw-rw-   0        0        0      239 2023-06-01 19:38:41.000000 oneoneoneexample-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 19:39:49.500258 oneoneoneexample-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      237 2023-05-31 21:36:29.000000 oneoneoneexample-0.7/setup.py
```

### Comparing `oneoneoneexample-0.6/pdf_generator/convert.py` & `oneoneoneexample-0.7/pdf_generator/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -147,9 +147,8 @@
     print(f'PDF file created: {merged_pdf_file}')
     print(f'Elapsed time: {elapsed_time / 60} minutes')
 
     # Delete the individual PDF files (optional)
     for pdf_file in pdf_files:
         os.remove(pdf_file)
 
-generate(json_file=r'C:\Users\Jigya\Downloads\new\actualData.json', template_directory=r'C:\Users\Jigya\Downloads\new', output_html_path=r'C:\Users\Jigya\Downloads\new', new_pdf_path=r'C:\Users\Jigya\Downloads\new')
```

