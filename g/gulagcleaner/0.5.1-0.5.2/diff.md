# Comparing `tmp/gulagcleaner-0.5.1.tar.gz` & `tmp/gulagcleaner-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.5.1.tar", last modified: Wed May 31 21:42:51 2023, max compression
+gzip compressed data, was "gulagcleaner-0.5.2.tar", last modified: Wed May 31 22:42:56 2023, max compression
```

## Comparing `gulagcleaner-0.5.1.tar` & `gulagcleaner-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.379112 gulagcleaner-0.5.1/
--rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     2437 2023-05-31 21:42:51.379112 gulagcleaner-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2023-05-31 21:24:37.000000 gulagcleaner-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.349077 gulagcleaner-0.5.1/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     2757 2023-05-31 21:39:11.000000 gulagcleaner-0.5.1/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0     5889 2023-05-31 21:40:21.000000 gulagcleaner-0.5.1/gulagcleaner/gulagcleaner_extract.py
-drwxrwxrwx   0        0        0        0 2023-05-31 21:42:51.377076 gulagcleaner-0.5.1/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     2437 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-31 21:42:51.000000 gulagcleaner-0.5.1/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      857 2023-05-31 21:42:51.386081 gulagcleaner-0.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.117352 gulagcleaner-0.5.2/
+-rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0     2437 2023-05-31 22:42:56.117352 gulagcleaner-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2023-05-31 21:58:02.000000 gulagcleaner-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.087160 gulagcleaner-0.5.2/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-05-31 22:41:03.000000 gulagcleaner-0.5.2/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0     5926 2023-05-31 22:40:26.000000 gulagcleaner-0.5.2/gulagcleaner/gulagcleaner_extract.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:42:56.115474 gulagcleaner-0.5.2/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     2437 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 22:42:56.000000 gulagcleaner-0.5.2/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      857 2023-05-31 22:42:56.120348 gulagcleaner-0.5.2/setup.cfg
```

### Comparing `gulagcleaner-0.5.1/LICENSE` & `gulagcleaner-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.5.1/PKG-INFO` & `gulagcleaner-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.1
+Version: 0.5.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162,KosmicKatXV,pgalinanes
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 Gulag Cleaner can be used through both a Command Line Interface (CLI) and in your code.
 
 ### Command Line Interface
 
 To use Gulag Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of your PDF file:
 
 ```
-gulagcleaner <filename> [-r] [-h] [-o] [-v]
+gulagcleaner [-r] [-h] [-o] [-v] <filename>
 ```
 
 ### Code
 
 To use Gulag Cleaner in your code, you can use the following code snippet:
 
 ```python
```

### Comparing `gulagcleaner-0.5.1/README.md` & `gulagcleaner-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Gulag Cleaner can be used through both a Command Line Interface (CLI) and in your code.
 
 ### Command Line Interface
 
 To use Gulag Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of your PDF file:
 
 ```
-gulagcleaner <filename> [-r] [-h] [-o] [-v]
+gulagcleaner [-r] [-h] [-o] [-v] <filename>
 ```
 
 ### Code
 
 To use Gulag Cleaner in your code, you can use the following code snippet:
 
 ```python
```

### Comparing `gulagcleaner-0.5.1/gulagcleaner/command_line.py` & `gulagcleaner-0.5.2/gulagcleaner/command_line.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
         print("")
         print("Deembeds pages from a PDF file.")
         print("")
         print("Positional arguments:")
         print("  filename      the PDF file to deembed pages from.")
         print("")
         print("Optional arguments:")
-        print("  -h            show this help message and exit.")
+        print("  -h            show this help message.")
         print("  -r            replaces the original file with the deembedded file.")
         print("  -o            uses the old deembeding method (for files older than 18/05/2023).")
         print("  -v            shows the version of the program.")
         return
 
     # Check for the -v argument
     if '-v' in sys.argv:
-        print("actual version: 0.5.1")
+        print("actual version: 0.5.2")
         return
 
     # Get the filename argument
     if len(sys.argv) < 2:
         print('Usage: gulagcleaner [-h] [-r] [-o] [-v] <filename>')
         return
     filename = sys.argv[-1]
```

### Comparing `gulagcleaner-0.5.1/gulagcleaner/gulagcleaner_extract.py` & `gulagcleaner-0.5.2/gulagcleaner/gulagcleaner_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,14 +120,15 @@
                     pares = find_iobj_pairs(content_list[i], content_list[i + 1])
                 new_contents.append(pares[0][pares[1]-2:pares[1]+6])
 
             newpages = []
             for i,page in enumerate([page for page in pdf.pages if len(page.Contents)>1]):
                 newpage = page.copy()
                 newpage.Contents = [pdf.indirect_objects[iobj] for iobj in new_contents[i]]
+                newpage.Annots = []
                 newpages.append(newpage)
         else:
             os.remove(intermediate_pdf_path)
             return {
                 "Success": False,
                 "return_path": "",
                 "Error": "Deembeding method not found.",
```

### Comparing `gulagcleaner-0.5.1/gulagcleaner.egg-info/PKG-INFO` & `gulagcleaner-0.5.2/gulagcleaner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulagcleaner
-Version: 0.5.1
+Version: 0.5.2
 Summary: Ad removal tool for PDFs written in python.
 Home-page: https://github.com/YM162/gulag-cleaner-cli
 Author: YM162,KosmicKatXV,pgalinanes
 Author-email: david.fontaneda16@gmail.com
 Project-URL: Bug Tracker, https://github.com/YM162/gulag-cleaner-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 Gulag Cleaner can be used through both a Command Line Interface (CLI) and in your code.
 
 ### Command Line Interface
 
 To use Gulag Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of your PDF file:
 
 ```
-gulagcleaner <filename> [-r] [-h] [-o] [-v]
+gulagcleaner [-r] [-h] [-o] [-v] <filename>
 ```
 
 ### Code
 
 To use Gulag Cleaner in your code, you can use the following code snippet:
 
 ```python
```

### Comparing `gulagcleaner-0.5.1/setup.cfg` & `gulagcleaner-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e31  .version = 0.5.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e32  .version = 0.5.2
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 2c4b 6f73 6d69 634b 6174 5856 2c70 6761  ,KosmicKatXV,pga
 00000050: 6c69 6e61 6e65 730d 0a61 7574 686f 725f  linanes..author_
 00000060: 656d 6169 6c20 3d20 6461 7669 642e 666f  email = david.fo
 00000070: 6e74 616e 6564 6131 3640 676d 6169 6c2e  ntaneda16@gmail.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 6420 7265 6d6f 7661 6c20 746f   = Ad removal to
```

