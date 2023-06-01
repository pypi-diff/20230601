# Comparing `tmp/anonupload-1.1.6-py3-none-any.whl.zip` & `tmp/anonupload-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6105 bytes, number of entries: 8
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:27 anonupload/__init__.py
--rw-r--r--  2.0 unx     7091 b- defN 23-May-26 14:27 anonupload/main.py
--rwxr-xr-x  2.0 unx     1064 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2529 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-May-26 14:28 anonupload-1.1.6.dist-info/RECORD
-8 files, 11576 bytes uncompressed, 4961 bytes compressed:  57.1%
+Zip file size: 6113 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 05:51 anonupload/__init__.py
+-rw-r--r--  2.0 unx     7107 b- defN 23-Jun-01 05:51 anonupload/main.py
+-rwxr-xr-x  2.0 unx     1064 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2529 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      651 b- defN 23-Jun-01 05:51 anonupload-1.1.7.dist-info/RECORD
+8 files, 11592 bytes uncompressed, 4969 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: anonupload/__init__.py
 Comment: 
 
 Filename: anonupload/main.py
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/LICENSE
+Filename: anonupload-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/METADATA
+Filename: anonupload-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/WHEEL
+Filename: anonupload-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/entry_points.txt
+Filename: anonupload-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/top_level.txt
+Filename: anonupload-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: anonupload-1.1.6.dist-info/RECORD
+Filename: anonupload-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anonupload/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 
 from .main import download, downloads, upload, changefile_and_upload
```

## anonupload/main.py

```diff
@@ -190,15 +190,15 @@
 	first_msg, second_msg = upload(full_filename)
 	if delete:
 		remove_file(full_filename)
 	return first_msg, second_msg
 
 def downloads(urls: List[str], path: Path=Path.cwd(), delete: bool=False):
 	for url in urls:
-		download(url, path, delete)
+		download(url=url, path=path, delete=delete)
 	
 example_uses = '''example:
    anon up {files_name}
    anon d {urls}'''
 
 def main(argv = None):
 	parser = argparse.ArgumentParser(prog=package_name, description="upload your files on anonfile server", epilog=example_uses, formatter_class=argparse.RawDescriptionHelpFormatter)
```

## Comparing `anonupload-1.1.6.dist-info/LICENSE` & `anonupload-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `anonupload-1.1.6.dist-info/METADATA` & `anonupload-1.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonupload
-Version: 1.1.6
+Version: 1.1.7
 Summary: upload and download to anonfiles server
 Home-page: https://github.com/jakbin/anonupload
 Author: Jak Bin
 Author-email: jakbin4747@gmail.com
 Project-URL: Bug Tracker, https://github.com/jakbin/anonupload/issues
 Keywords: anonfile,anonfile-api,anonfile-cli,anonymous,upload
 Classifier: Programming Language :: Python :: 3.6
```

