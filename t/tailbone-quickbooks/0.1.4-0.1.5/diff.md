# Comparing `tmp/tailbone-quickbooks-0.1.4.tar.gz` & `tmp/tailbone-quickbooks-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tailbone-quickbooks-0.1.4.tar", last modified: Wed Feb 22 01:17:59 2023, max compression
+gzip compressed data, was "dist/tailbone-quickbooks-0.1.5.tar", last modified: Thu Jun  1 19:30:50 2023, max compression
```

## Comparing `tailbone-quickbooks-0.1.4.tar` & `tailbone-quickbooks-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/
--rw-r--r--   0 lance     (1000) lance     (1000)       82 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.4/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     3601 2022-12-08 23:38:00.000000 tailbone-quickbooks-0.1.4/setup.py
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/setup.cfg
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exportable-invoices/
--rw-r--r--   0 lance     (1000) lance     (1000)      796 2022-12-21 01:36:38.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exportable-invoices/view.mako
--rw-r--r--   0 lance     (1000) lance     (1000)     4095 2023-01-11 14:20:02.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exportable-invoices/index.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exports/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exports/invoice/
--rw-r--r--   0 lance     (1000) lance     (1000)      299 2022-12-20 20:48:41.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exports/invoice/view.mako
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/
--rw-r--r--   0 lance     (1000) lance     (1000)     1682 2022-12-21 01:24:12.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1937 2022-12-21 01:34:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/vendors.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/quickbooks/
--rw-r--r--   0 lance     (1000) lance     (1000)    19725 2023-02-22 00:48:37.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/quickbooks/invoices.py
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-12-09 05:45:04.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/quickbooks/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1890 2022-12-09 04:57:20.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/departments.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1170 2022-12-21 01:24:18.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-02-22 01:17:27.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/_version.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1011 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      782 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       28 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       20 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)     1099 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      350 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.4/README.rst
--rw-r--r--   0 lance     (1000) lance     (1000)      853 2023-02-22 01:17:23.000000 tailbone-quickbooks-0.1.4/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)     1099 2023-02-22 01:17:59.000000 tailbone-quickbooks-0.1.4/PKG-INFO
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/
+-rw-r--r--   0 lance     (1000) lance     (1000)       82 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.5/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1015 2023-05-16 19:34:58.000000 tailbone-quickbooks-0.1.5/setup.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      822 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/setup.cfg
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exportable-invoices/
+-rw-r--r--   0 lance     (1000) lance     (1000)      796 2022-12-21 01:36:38.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exportable-invoices/view.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)     4095 2023-01-11 14:20:02.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exportable-invoices/index.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exports/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exports/invoice/
+-rw-r--r--   0 lance     (1000) lance     (1000)      299 2022-12-20 20:48:41.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exports/invoice/view.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1682 2022-12-21 01:24:12.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1937 2022-12-21 01:34:59.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/vendors.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/quickbooks/
+-rw-r--r--   0 lance     (1000) lance     (1000)    19699 2023-05-15 01:34:55.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/quickbooks/invoices.py
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2022-12-09 05:45:04.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/quickbooks/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1890 2022-12-09 04:57:20.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/departments.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1170 2022-12-21 01:24:18.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-06-01 19:30:36.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1011 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      792 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       28 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       20 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1099 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      350 2022-12-08 23:36:16.000000 tailbone-quickbooks-0.1.5/README.rst
+-rw-r--r--   0 lance     (1000) lance     (1000)      992 2023-06-01 19:30:31.000000 tailbone-quickbooks-0.1.5/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)     1099 2023-06-01 19:30:50.000000 tailbone-quickbooks-0.1.5/PKG-INFO
```

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exportable-invoices/view.mako` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exportable-invoices/view.mako`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/templates/quickbooks/exportable-invoices/index.mako` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/templates/quickbooks/exportable-invoices/index.mako`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/stores.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/stores.py`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/vendors.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/vendors.py`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/quickbooks/invoices.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/quickbooks/invoices.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     def select(self):
         """
         Mark one or more invoices as selected, within the current user's session.
         """
         model = self.model
 
         form = forms.Form(schema=ToggleInvoices(), request=self.request)
-        if not form.validate(newstyle=True):
+        if not form.validate():
             return {'error': "Form did not validate"}
         uuids = form.validated['uuids'].split(',')
 
         invoices = []
         for uuid in uuids:
             invoice = self.Session.get(model.QuickbooksExportableInvoice, uuid)
             if invoice and self.exportable(invoice):
@@ -364,15 +364,15 @@
     def deselect(self):
         """
         Mark one or more invoices as *not* selected, within the current user's session.
         """
         model = self.model
 
         form = forms.Form(schema=ToggleInvoices(), request=self.request)
-        if not form.validate(newstyle=True):
+        if not form.validate():
             return {'error': "Form did not validate"}
         uuids = form.validated['uuids'].split(',')
 
         invoices = []
         for uuid in uuids:
             invoice = self.Session.get(model.QuickbooksExportableInvoice, uuid)
             if invoice and self.exportable(invoice):
```

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/departments.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/departments.py`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/views/__init__.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/views/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks/__init__.py` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/SOURCES.txt` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGELOG.md
 MANIFEST.in
 README.rst
+setup.cfg
 setup.py
 tailbone_quickbooks/__init__.py
 tailbone_quickbooks/_version.py
 tailbone_quickbooks.egg-info/PKG-INFO
 tailbone_quickbooks.egg-info/SOURCES.txt
 tailbone_quickbooks.egg-info/dependency_links.txt
 tailbone_quickbooks.egg-info/requires.txt
```

### Comparing `tailbone-quickbooks-0.1.4/tailbone_quickbooks.egg-info/PKG-INFO` & `tailbone-quickbooks-0.1.5/tailbone_quickbooks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-quickbooks
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tailbone integration package for Quickbooks
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tailbone-quickbooks-0.1.4/CHANGELOG.md` & `tailbone-quickbooks-0.1.5/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 
 # Changelog
 All notable changes to tailbone-quickbooks will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [0.1.5] - 2023-06-01
+### Changed
+- Stop passing `newstyle` kwarg to `Form.validate()`.
+- Replace `setup.py` contents with `setup.cfg`.
+
 ## [0.1.4] - 2023-02-21
 ### Changed
 - Show invoice amounts as currency.
 
 ## [0.1.3] - 2023-02-20
 ### Changed
 - Refactor `Query.get()` => `Session.get()` per SQLAlchemy 1.4.
```

### Comparing `tailbone-quickbooks-0.1.4/PKG-INFO` & `tailbone-quickbooks-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tailbone-quickbooks
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tailbone integration package for Quickbooks
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

