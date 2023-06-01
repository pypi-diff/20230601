# Comparing `tmp/ngrok-0.8.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ngrok-0.8.1-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2392214 bytes, number of entries: 10
--rw-r--r--  4.6 unx     9950 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       53 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11558 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE
--rw-r--r--  4.6 unx     1056 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/license_files/LICENSE-MIT
--rw-r--r--  4.6 unx     5139 b- defN 23-May-19 21:52 ngrok/ngrok_parser.py
--rw-r--r--  4.6 unx      109 b- defN 23-May-19 21:52 ngrok/__init__.py
--rw-r--r--  4.6 unx     6527 b- defN 23-May-19 21:52 ngrok/__main__.py
--rwxr-xr-x  4.6 unx  6440960 b- defN 23-May-19 21:52 ngrok/ngrok.pyd
--rw-r--r--  4.6 unx      805 b- defN 23-May-19 21:52 ngrok-0.8.0.dist-info/RECORD
-10 files, 6476253 bytes uncompressed, 2390852 bytes compressed:  63.1%
+Zip file size: 2353978 bytes, number of entries: 10
+-rw-r--r--  4.6 unx     9950 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx       53 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11558 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/license_files/LICENSE-APACHE
+-rw-r--r--  4.6 unx     1056 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/license_files/LICENSE-MIT
+-rw-r--r--  4.6 unx     5139 b- defN 23-Jun-01 16:42 ngrok/ngrok_parser.py
+-rw-r--r--  4.6 unx      109 b- defN 23-Jun-01 16:42 ngrok/__init__.py
+-rw-r--r--  4.6 unx     6527 b- defN 23-Jun-01 16:42 ngrok/__main__.py
+-rwxr-xr-x  4.6 unx  6331904 b- defN 23-Jun-01 16:42 ngrok/ngrok.pyd
+-rw-r--r--  4.6 unx      805 b- defN 23-Jun-01 16:42 ngrok-0.8.1.dist-info/RECORD
+10 files, 6367197 bytes uncompressed, 2352616 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: ngrok-0.8.0.dist-info/METADATA
+Filename: ngrok-0.8.1.dist-info/METADATA
 Comment: 
 
-Filename: ngrok-0.8.0.dist-info/WHEEL
+Filename: ngrok-0.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: ngrok-0.8.0.dist-info/entry_points.txt
+Filename: ngrok-0.8.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE
+Filename: ngrok-0.8.1.dist-info/license_files/LICENSE-APACHE
 Comment: 
 
-Filename: ngrok-0.8.0.dist-info/license_files/LICENSE-MIT
+Filename: ngrok-0.8.1.dist-info/license_files/LICENSE-MIT
 Comment: 
 
 Filename: ngrok/ngrok_parser.py
 Comment: 
 
 Filename: ngrok/__init__.py
 Comment: 
 
 Filename: ngrok/__main__.py
 Comment: 
 
 Filename: ngrok/ngrok.pyd
 Comment: 
 
-Filename: ngrok-0.8.0.dist-info/RECORD
+Filename: ngrok-0.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ngrok-0.8.0.dist-info/METADATA` & `ngrok-0.8.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngrok
-Version: 0.8.0
+Version: 0.8.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Utilities
@@ -21,16 +21,16 @@
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: The ngrok Agent SDK for Python
 Keywords: ngrok,python,pypi,pyo3,ingress,networking
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://ngrok.com
 Project-URL: repository, https://github.com/ngrok/ngrok-python
+Project-URL: homepage, https://ngrok.com
 Project-URL: changelog, https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md
 
 # The ngrok Agent SDK for Python
 
 [![PyPI][pypi-badge]][pypi-url]
 [![Supported Versions][ver-badge]][ver-url]
 [![MIT licensed][mit-badge]][mit-url]
```

## Comparing `ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE` & `ngrok-0.8.1.dist-info/license_files/LICENSE-APACHE`

 * *Files identical despite different names*

## Comparing `ngrok-0.8.0.dist-info/license_files/LICENSE-MIT` & `ngrok-0.8.1.dist-info/license_files/LICENSE-MIT`

 * *Files identical despite different names*

## Comparing `ngrok-0.8.0.dist-info/RECORD` & `ngrok-0.8.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-ngrok-0.8.0.dist-info/METADATA,sha256=NrsvPHGOus_XldonFdfMBdolW5gS3bG2k6mLcOOK-FM,9950
-ngrok-0.8.0.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
-ngrok-0.8.0.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
-ngrok-0.8.0.dist-info/license_files/LICENSE-APACHE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ngrok-0.8.0.dist-info/license_files/LICENSE-MIT,sha256=k2H9oRPELrEi8YIKhwwvdIYmJTrpic5YINff621X-Fw,1056
+ngrok-0.8.1.dist-info/METADATA,sha256=0TRk-a7B-ztZ7kcdCkFrhJlE0DdcPyIX5AvYiF8PQAI,9950
+ngrok-0.8.1.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
+ngrok-0.8.1.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
+ngrok-0.8.1.dist-info/license_files/LICENSE-APACHE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+ngrok-0.8.1.dist-info/license_files/LICENSE-MIT,sha256=k2H9oRPELrEi8YIKhwwvdIYmJTrpic5YINff621X-Fw,1056
 ngrok/ngrok_parser.py,sha256=To2QN5nmRK_U0t4e_K3FtHwQDsIuhxfgMb3jar2FENc,5139
 ngrok/__init__.py,sha256=SVQFcbYIelbBItRJLTUbvEnhgLsOvauDlC3_hMuj-Ck,109
 ngrok/__main__.py,sha256=3W7zfMZKeAebaaLFZF9K9PQv25K1vMr7YM8lsN6TzCI,6527
-ngrok/ngrok.pyd,sha256=Xa8qbS97jdjnZTPp59AjVejXvz6h2mmtwnW3mJc_teo,6440960
-ngrok-0.8.0.dist-info/RECORD,,
+ngrok/ngrok.pyd,sha256=uJfepTHnkEENvcZ5xDVYhr-iEcVtXg-L388Q4MMjYRE,6331904
+ngrok-0.8.1.dist-info/RECORD,,
```

