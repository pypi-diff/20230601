# Comparing `tmp/web_data_extraction-0.0.1.tar.gz` & `tmp/web_data_extraction-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_data_extraction-0.0.1.tar", max compression
+gzip compressed data, was "web_data_extraction-0.0.2.tar", max compression
```

## Comparing `web_data_extraction-0.0.1.tar` & `web_data_extraction-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      667 2023-05-31 13:13:20.844972 web_data_extraction-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      804 2023-05-31 09:56:37.956991 web_data_extraction-0.0.1/README.md
--rw-r--r--   0        0        0       57 2023-05-31 09:04:40.848747 web_data_extraction-0.0.1/web_data_extraction/__init__.py
--rw-r--r--   0        0        0    13458 2023-05-31 09:00:33.460362 web_data_extraction-0.0.1/web_data_extraction/web_data_extraction.py
--rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 web_data_extraction-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      671 2023-06-01 14:33:28.881893 web_data_extraction-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-05-31 09:56:37.956991 web_data_extraction-0.0.2/README.md
+-rw-r--r--   0        0        0       57 2023-05-31 09:04:40.848747 web_data_extraction-0.0.2/web_data_extraction/__init__.py
+-rw-r--r--   0        0        0    13467 2023-06-01 12:06:03.715243 web_data_extraction-0.0.2/web_data_extraction/web_data_extraction.py
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 web_data_extraction-0.0.2/PKG-INFO
```

### Comparing `web_data_extraction-0.0.1/pyproject.toml` & `web_data_extraction-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "web-data-extraction"
-version = "0.0.1"
+version = "0.0.2"
 description = "A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent"
-authors = ["Lisa Yvette INYANGE <inyangel@yahoo.com>"]
+authors = ["Lisa Yvette INYANGE <linyange@andrew.cmu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ILisa250/web-data-extraction"
 repository = "https://github.com/ILisa250/web-data-extraction"
 keywords = ["web-data-extraction", "web-scraping", "Lisa"]
 
 packages = [{include = "web_data_extraction"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `web_data_extraction-0.0.1/README.md` & `web_data_extraction-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `web_data_extraction-0.0.1/web_data_extraction/web_data_extraction.py` & `web_data_extraction-0.0.2/web_data_extraction/web_data_extraction.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 # Modules to run automatically
 import schedule # To handle scheduling tasks.
 import time as tm # For time-related operations
 
 
 run_count = 0  # Counter for tracking the number of times the script has run
-def scrape_and_clean_data_appart4sale():
+def scrape_and_clean_data_appart4sale(filename):
     global run_count
     run_count += 1
     current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
     
 
     def get_real_estate_data(filename):
@@ -273,26 +273,27 @@
         conn.close()
 
 
     # Function to combine all the functions into one
     #...............................................
     def combined_function():
         # URL of the real estate listings page on 'imali.biz', with the page number left blank 
-        imali_data = get_real_estate_data(filename = 'https://imali.biz/category/1/125/search?pg=')
+        imali_data = get_real_estate_data(filename)
         extract_appart4sale_data()
         clean_and_save_appart4sale_data()
         # Specify the path to the CSV file
         csv_file_path = 'C:\\Users\\yinyange\\Documents\\BNR\\Imali_properties\\House&Appart(all)\\Appart4sale(all)\\IMALI_apartment4sale_Clean_data.csv'
         # Insert data from the CSV file to the table
-        insert_data_from_csv_to_imali_table(csv_file_path)
+#         insert_data_from_csv_to_imali_table(csv_file_path)
 
     # Call the combined function
     combined_function()
     print(f"Script has run {run_count} times. Current time: {current_time}\n\n")
-scrape_and_clean_data_appart4sale()   
+scrape_and_clean_data_appart4sale('https://imali.biz/category/1/125/search?pg=')   
+
 
     
 # Automation
 # ..........
 # # ..........
 # schedule.every(5).minutes.do(scrape_and_clean_data_appart4sale)
```

### Comparing `web_data_extraction-0.0.1/PKG-INFO` & `web_data_extraction-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: web-data-extraction
-Version: 0.0.1
+Version: 0.0.2
 Summary: A unified collection of web data premises eg Apartment for sale, apartment for rent, house for sale, house for rent
 Home-page: https://github.com/ILisa250/web-data-extraction
 License: MIT
 Keywords: web-data-extraction,web-scraping,Lisa
 Author: Lisa Yvette INYANGE
-Author-email: inyangel@yahoo.com
-Requires-Python: >=3.10,<4.0
+Author-email: linyange@andrew.cmu.edu
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/ILisa250/web-data-extraction
 Description-Content-Type: text/markdown
 
 A unified scraper collection of web data
```

