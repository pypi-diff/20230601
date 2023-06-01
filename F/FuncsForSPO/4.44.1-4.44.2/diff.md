# Comparing `tmp/FuncsForSPO-4.44.1.tar.gz` & `tmp/FuncsForSPO-4.44.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.44.1.tar", last modified: Fri May 26 15:54:54 2023, max compression
+gzip compressed data, was "FuncsForSPO-4.44.2.tar", last modified: Thu Jun  1 11:59:18 2023, max compression
```

## Comparing `FuncsForSPO-4.44.1.tar` & `FuncsForSPO-4.44.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.859940 FuncsForSPO-4.44.1/
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.513900 FuncsForSPO-4.44.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.569182 FuncsForSPO-4.44.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.44.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.44.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.579816 FuncsForSPO-4.44.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.44.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.589146 FuncsForSPO-4.44.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.44.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.599281 FuncsForSPO-4.44.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.44.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.506297 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.616294 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.636472 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.643168 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.661363 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5054 2023-05-26 15:54:29.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.672397 FuncsForSPO-4.44.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.715593 FuncsForSPO-4.44.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-4.44.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.732724 FuncsForSPO-4.44.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.44.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.744518 FuncsForSPO-4.44.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.44.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.754875 FuncsForSPO-4.44.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.44.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.763323 FuncsForSPO-4.44.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.44.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.44.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.768417 FuncsForSPO-4.44.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.44.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:54:54.559307 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-05-26 15:54:54.000000 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-05-26 15:54:54.000000 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:54:54.000000 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-05-26 15:54:54.000000 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-05-26 15:54:54.000000 FuncsForSPO-4.44.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.44.1/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-05-26 15:54:54.854972 FuncsForSPO-4.44.1/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.44.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 15:54:54.859940 FuncsForSPO-4.44.1/setup.cfg
--rw-rw-rw-   0        0        0     2177 2023-05-26 15:54:45.000000 FuncsForSPO-4.44.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.416564 FuncsForSPO-4.44.2/
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:17.941861 FuncsForSPO-4.44.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.044283 FuncsForSPO-4.44.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.44.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.44.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.059910 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.076741 FuncsForSPO-4.44.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.44.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.091910 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:17.931086 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.114232 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.147309 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.158227 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.182931 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9918 2023-06-01 11:55:59.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.202973 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.253542 FuncsForSPO-4.44.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.275635 FuncsForSPO-4.44.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.44.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.291670 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.309305 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.324150 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.336515 FuncsForSPO-4.44.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.44.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.020959 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8027 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1331 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      350 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.44.2/LICENSE
+-rw-rw-rw-   0        0        0     8027 2023-06-01 11:59:18.411051 FuncsForSPO-4.44.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.44.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:59:18.417569 FuncsForSPO-4.44.2/setup.cfg
+-rw-rw-rw-   0        0        0     2177 2023-06-01 11:59:05.000000 FuncsForSPO-4.44.2/setup.py
```

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-4.44.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,24 +177,27 @@
                         else:
                             wait=False
                             sleep(3)
                             if prints:
                                 print('OCR Concluido!')
             verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
         except Exception as e:
-            print('Ocorreu um erro!')
-            print(str(e))
-            
+            self.DRIVER.quit()
+            faz_log(f'Ocorreu um erro: {repr(e)}', 'c*')
+
 
-            
     def recupera_texto(self) -> str:
-        if self.get_text_into_code:
-            try:
-                file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
-                file_txt = file_txts[-1]
-                text = None
-                with open(file_txt, mode='r', encoding='utf-16-le') as f:
-                    text = f.read()
-                shutil.rmtree(self.DOWNLOAD_DIR)
-                return text
-            except IndexError:
-                raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
+        try:
+            if self.get_text_into_code:
+                try:
+                    file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
+                    file_txt = file_txts[-1]
+                    text = None
+                    with open(file_txt, mode='r', encoding='utf-16-le') as f:
+                        text = f.read()
+                    shutil.rmtree(self.DOWNLOAD_DIR)
+                    return text
+                except IndexError:
+                    raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
+        except Exception:
+            self.DRIVER.quit()
+            raise FalhaAoRecuperarOcr(f'Ocorreu um erro na recuperação que causou um Exception: {repr(e)}')
```

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,20 +122,20 @@
             # Define o corpo da solicitação com o ID do trabalho de OCR
             if clear_task:
                 params = {'id': id_, 'delete':'True'}
             else:
                 params = {'id': id_, 'delete':'False'}
             data = json.dumps(params)
             # Envia a solicitação HTTP POST com o corpo JSON
+            sleep(sleep_for_request)
             response = requests.post(url, data=data, headers={'Content-Type': 'application/json'})
 
             # Extrai o texto da resposta JSON
             try:
                 response_json = response.json()
             except Exception as e:
                 print(e)
                 raise ErroAPI('ErroAPI')
             if response_json.get('status') == 'finalizado':
                 return response_json.get('result')
             else:
                 print(response_json.get('status'))
-                sleep(sleep_for_request)
```

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-4.44.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-4.44.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.44.1
+Version: 4.44.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.44.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-4.44.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/LICENSE` & `FuncsForSPO-4.44.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/PKG-INFO` & `FuncsForSPO-4.44.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.44.1
+Version: 4.44.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.44.1/README.md` & `FuncsForSPO-4.44.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.1/setup.py` & `FuncsForSPO-4.44.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.44.1'
+version = '4.44.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

