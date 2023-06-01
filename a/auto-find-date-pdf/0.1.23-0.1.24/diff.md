# Comparing `tmp/auto_find_date_pdf-0.1.23.tar.gz` & `tmp/auto_find_date_pdf-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_find_date_pdf-0.1.23.tar", last modified: Thu May 11 02:27:25 2023, max compression
+gzip compressed data, was "auto_find_date_pdf-0.1.24.tar", last modified: Thu Jun  1 02:02:09 2023, max compression
```

## Comparing `auto_find_date_pdf-0.1.23.tar` & `auto_find_date_pdf-0.1.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/
--rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.23/LICENSE
--rw-rw-rw-   0        0        0     2077 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/PKG-INFO
--rw-rw-rw-   0        0        0     1781 2023-05-10 20:43:13.000000 auto_find_date_pdf-0.1.23/README.md
--rw-rw-rw-   0        0        0        0 2023-05-10 20:30:13.000000 auto_find_date_pdf-0.1.23/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 02:27:25.061061 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/
--rw-rw-rw-   0        0        0     2077 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-05-11 02:27:25.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-11 02:27:24.000000 auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      920 2023-05-11 00:11:23.000000 auto_find_date_pdf-0.1.23/main.py
--rw-rw-rw-   0        0        0       42 2023-05-11 02:27:25.062064 auto_find_date_pdf-0.1.23/setup.cfg
--rw-rw-rw-   0        0        0      732 2023-05-11 02:27:14.000000 auto_find_date_pdf-0.1.23/setup.py
--rw-rw-rw-   0        0        0     2227 2023-04-24 03:02:35.000000 auto_find_date_pdf-0.1.23/test_fast.py
--rw-rw-rw-   0        0        0     6858 2023-04-24 03:24:11.000000 auto_find_date_pdf-0.1.23/text_search.py
+drwxrwxrwx   0        0        0        0 2023-06-01 02:02:09.042562 auto_find_date_pdf-0.1.24/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 05:51:11.000000 auto_find_date_pdf-0.1.24/LICENSE
+-rw-rw-rw-   0        0        0     2077 2023-06-01 02:02:09.042562 auto_find_date_pdf-0.1.24/PKG-INFO
+-rw-rw-rw-   0        0        0     1781 2023-05-10 20:43:13.000000 auto_find_date_pdf-0.1.24/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-10 20:30:13.000000 auto_find_date_pdf-0.1.24/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-01 02:02:09.041532 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/
+-rw-rw-rw-   0        0        0     2077 2023-06-01 02:02:08.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-01 02:02:09.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 02:02:08.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-01 02:02:08.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-01 02:02:08.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-01 02:02:08.000000 auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      920 2023-05-11 00:11:23.000000 auto_find_date_pdf-0.1.24/main.py
+-rw-rw-rw-   0        0        0       42 2023-06-01 02:02:09.042562 auto_find_date_pdf-0.1.24/setup.cfg
+-rw-rw-rw-   0        0        0      732 2023-06-01 02:01:49.000000 auto_find_date_pdf-0.1.24/setup.py
+-rw-rw-rw-   0        0        0     2227 2023-04-24 03:02:35.000000 auto_find_date_pdf-0.1.24/test_fast.py
+-rw-rw-rw-   0        0        0     7010 2023-06-01 02:01:07.000000 auto_find_date_pdf-0.1.24/text_search.py
```

### Comparing `auto_find_date_pdf-0.1.23/LICENSE` & `auto_find_date_pdf-0.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.23/PKG-INFO` & `auto_find_date_pdf-0.1.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_find_date_pdf
-Version: 0.1.23
+Version: 0.1.24
 Summary: A simple lib to find dates from any txt/ pdf/ rtf source. For documentation see
 Author: Your Name
 Author-email: opensource@marvsai.com
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Simple use Date and text parsing from pdf rtf and images (with use of call back function)
```

### Comparing `auto_find_date_pdf-0.1.23/README.md` & `auto_find_date_pdf-0.1.24/README.md`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.23/auto_find_date_pdf.egg-info/PKG-INFO` & `auto_find_date_pdf-0.1.24/auto_find_date_pdf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-find-date-pdf
-Version: 0.1.23
+Version: 0.1.24
 Summary: A simple lib to find dates from any txt/ pdf/ rtf source. For documentation see
 Author: Your Name
 Author-email: opensource@marvsai.com
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Simple use Date and text parsing from pdf rtf and images (with use of call back function)
```

### Comparing `auto_find_date_pdf-0.1.23/main.py` & `auto_find_date_pdf-0.1.24/main.py`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.23/setup.py` & `auto_find_date_pdf-0.1.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 read_md = lambda f: open(f, 'r').read()
 
 setup(
     name='auto_find_date_pdf',
-    version='0.1.23',
+    version='0.1.24',
     description='A simple lib to find dates from any txt/ pdf/ rtf source. For documentation see',
     long_description=read_md('README.md'),
     long_description_content_type="text/markdown; charset=UTF-8",
     author='Your Name',
 
     author_email='opensource@marvsai.com',
     packages=find_packages(exclude=['test_fast*']),
```

### Comparing `auto_find_date_pdf-0.1.23/test_fast.py` & `auto_find_date_pdf-0.1.24/test_fast.py`

 * *Files identical despite different names*

### Comparing `auto_find_date_pdf-0.1.23/text_search.py` & `auto_find_date_pdf-0.1.24/text_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,20 +76,23 @@
             try:
                 date = datetime.strptime(match, '%m/%d/%Y')
             except ValueError:
                 try:
                     date = datetime.strptime(match, '%d/%m/%Y')
                 except ValueError:
                     try:
-                        date = datetime.strptime(match, '%m-%d-%Y')
-                    except ValueError:
+                        date = datetime.strptime(match, '%d/%m/%y')
+                    except:
                         try:
-                            date = datetime.strptime(match, '%d-%m-%Y')
+                            date = datetime.strptime(match, '%m-%d-%Y')
                         except ValueError:
-                            date = None
+                            try:
+                                date = datetime.strptime(match, '%d-%m-%Y')
+                            except ValueError:
+                                date = None
         if date is not None:
             dates.append(date)
 
 
 def find_dates(file_contents: str):
     """
       Find any dates in a large python string usually taken from a file or pdf
```

