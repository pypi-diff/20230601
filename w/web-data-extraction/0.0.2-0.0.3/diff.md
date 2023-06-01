# Comparing `tmp/web_data_extraction-0.0.2.tar.gz` & `tmp/web_data_extraction-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_data_extraction-0.0.2.tar", max compression
+gzip compressed data, was "web_data_extraction-0.0.3.tar", max compression
```

## Comparing `web_data_extraction-0.0.2.tar` & `web_data_extraction-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      671 2023-06-01 14:33:28.881893 web_data_extraction-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      804 2023-05-31 09:56:37.956991 web_data_extraction-0.0.2/README.md
--rw-r--r--   0        0        0       57 2023-05-31 09:04:40.848747 web_data_extraction-0.0.2/web_data_extraction/__init__.py
--rw-r--r--   0        0        0    13467 2023-06-01 12:06:03.715243 web_data_extraction-0.0.2/web_data_extraction/web_data_extraction.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 web_data_extraction-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      671 2023-06-01 14:42:19.837208 web_data_extraction-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-05-31 09:56:37.956991 web_data_extraction-0.0.3/README.md
+-rw-r--r--   0        0        0       57 2023-05-31 09:04:40.848747 web_data_extraction-0.0.3/web_data_extraction/__init__.py
+-rw-r--r--   0        0        0    13469 2023-06-01 14:41:40.460363 web_data_extraction-0.0.3/web_data_extraction/web_data_extraction.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 web_data_extraction-0.0.3/PKG-INFO
```

### Comparing `web_data_extraction-0.0.2/pyproject.toml` & `web_data_extraction-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-data-extraction"
-version = "0.0.2"
+version = "0.0.3"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
 authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/web-data-extraction"
 repository = "https://github.com/ILisa250/web-data-extraction"
 keywords = ["web-data-extraction", "web-scraping", "Lisa"]
```

### Comparing `web_data_extraction-0.0.2/README.md` & `web_data_extraction-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `web_data_extraction-0.0.2/web_data_extraction/web_data_extraction.py` & `web_data_extraction-0.0.3/web_data_extraction/web_data_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         csv_file_path = 'C:\\Users\\yinyange\\Documents\\BNR\\Imali_properties\\House&Appart(all)\\Appart4sale(all)\\IMALI_apartment4sale_Clean_data.csv'
         # Insert data from the CSV file to the table
 #         insert_data_from_csv_to_imali_table(csv_file_path)
 
     # Call the combined function
     combined_function()
     print(f"Script has run {run_count} times. Current time: {current_time}\n\n")
-scrape_and_clean_data_appart4sale('https://imali.biz/category/1/125/search?pg=')   
+# scrape_and_clean_data_appart4sale('https://imali.biz/category/1/125/search?pg=')   
 
 
     
 # Automation
 # ..........
 # # ..........
 # schedule.every(5).minutes.do(scrape_and_clean_data_appart4sale)
```

### Comparing `web_data_extraction-0.0.2/PKG-INFO` & `web_data_extraction-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-data-extraction
-Version: 0.0.2
+Version: 0.0.3
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/web-data-extraction
 License: MIT
 Keywords: web-data-extraction,web-scraping,Lisa
 Author: Lisa Yvette INYANGE
 Author-email: linyange@andrew.cmu.edu
 Requires-Python: >=3.9,<4.0
```

