# Comparing `tmp/ibonds-1.0.1.tar.gz` & `tmp/ibonds-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibonds-1.0.1.tar", last modified: Sat Apr 29 23:52:47 2023, max compression
+gzip compressed data, was "ibonds-1.0.2.tar", last modified: Thu Jun  1 03:15:52 2023, max compression
```

## Comparing `ibonds-1.0.1.tar` & `ibonds-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.983502 ibonds-1.0.1/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.1/LICENSE
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.1/MANIFEST.in
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-29 23:52:47.980169 ibonds-1.0.1/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.1/README.md
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/ibonds/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6966 2023-04-11 05:01:51.000000 ibonds-1.0.1/ibonds/__init__.py
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1328 2023-04-29 00:47:18.000000 ibonds-1.0.1/ibonds/interest_rates.yaml
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/ibonds.egg-info/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1854 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/PKG-INFO
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/SOURCES.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/dependency_links.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/requires.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2023-04-29 23:52:47.000000 ibonds-1.0.1/ibonds.egg-info/top_level.txt
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-04-29 23:52:47.983502 ibonds-1.0.1/setup.cfg
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1004 2023-04-29 23:52:21.000000 ibonds-1.0.1/setup.py
-drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-04-29 23:52:47.980169 ibonds-1.0.1/tests/
--rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5108 2023-04-29 00:54:03.000000 ibonds-1.0.1/tests/test_ibonds.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-06-01 03:15:52.298851 ibonds-1.0.2/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1071 2023-04-03 03:32:07.000000 ibonds-1.0.2/LICENSE
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       35 2023-04-11 04:27:26.000000 ibonds-1.0.2/MANIFEST.in
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1863 2023-06-01 03:15:52.298851 ibonds-1.0.2/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1311 2023-04-11 04:42:03.000000 ibonds-1.0.2/README.md
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-06-01 03:15:52.298851 ibonds-1.0.2/ibonds/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     6966 2023-06-01 03:12:33.000000 ibonds-1.0.2/ibonds/__init__.py
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1328 2023-04-29 00:47:18.000000 ibonds-1.0.2/ibonds/interest_rates.yaml
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-06-01 03:15:52.298851 ibonds-1.0.2/ibonds.egg-info/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1863 2023-06-01 03:15:52.000000 ibonds-1.0.2/ibonds.egg-info/PKG-INFO
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)      254 2023-06-01 03:15:52.000000 ibonds-1.0.2/ibonds.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        1 2023-06-01 03:15:52.000000 ibonds-1.0.2/ibonds.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       27 2023-06-01 03:15:52.000000 ibonds-1.0.2/ibonds.egg-info/requires.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)        7 2023-06-01 03:15:52.000000 ibonds-1.0.2/ibonds.egg-info/top_level.txt
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)       38 2023-06-01 03:15:52.298851 ibonds-1.0.2/setup.cfg
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     1013 2023-06-01 03:15:30.000000 ibonds-1.0.2/setup.py
+drwxr-xr-x   0 sarvjeet  (1000) sarvjeet  (1000)        0 2023-06-01 03:15:52.298851 ibonds-1.0.2/tests/
+-rw-r--r--   0 sarvjeet  (1000) sarvjeet  (1000)     5167 2023-06-01 03:10:53.000000 ibonds-1.0.2/tests/test_ibonds.py
```

### Comparing `ibonds-1.0.1/LICENSE` & `ibonds-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.1/PKG-INFO` & `ibonds-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.1
-Summary: Library to calculate the current value of a Series I savings bond
+Version: 1.0.2
+Summary: Library to calculate the current value of a Series I Savings bond (I Bond)
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ibonds-1.0.1/README.md` & `ibonds-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.1/ibonds/__init__.py` & `ibonds-1.0.2/ibonds/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
                                                  self.issue_date.month))
         rate_change_month = current_month + (- (age_months % 6))
         return self.interest_rates.composite_rate(self.fixed_rate(),
                                                   rate_change_month.date())
 
     def value(self, d=date.today()):
         """Returns value of this I Bond on date d."""
-        assert (d - self.issue_date) >= timedelta(days=1), (
+        assert (d - self.issue_date) >= timedelta(days=0), (
             f'Cannot compute value on {d} which is before the issue date '
             f'{self.issue_date}')
 
         # All bond values are multiple of $25 bond.
         value_25 = 25.0
         value_on = _YearMonth(self.issue_date.year, self.issue_date.month)
         months_left = _YearMonth(d.year, d.month) - value_on
```

### Comparing `ibonds-1.0.1/ibonds/interest_rates.yaml` & `ibonds-1.0.2/ibonds/interest_rates.yaml`

 * *Files identical despite different names*

### Comparing `ibonds-1.0.1/ibonds.egg-info/PKG-INFO` & `ibonds-1.0.2/ibonds.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ibonds
-Version: 1.0.1
-Summary: Library to calculate the current value of a Series I savings bond
+Version: 1.0.2
+Summary: Library to calculate the current value of a Series I Savings bond (I Bond)
 Home-page: https://github.com/sarvjeets/ibonds
 Author: Sarvjeet Singh
 Author-email: sarvjeet@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ibonds-1.0.1/setup.py` & `ibonds-1.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='ibonds',
-    version='1.0.1',
+    version='1.0.2',
     author='Sarvjeet Singh',
     author_email='sarvjeet@gmail.com',
     description=('Library to calculate the current value of a '
-                 'Series I savings bond'),
+                 'Series I Savings bond (I Bond)'),
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sarvjeets/ibonds',
     license="MIT",
     platforms='any',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `ibonds-1.0.1/tests/test_ibonds.py` & `ibonds-1.0.2/tests/test_ibonds.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
         with self.assertRaisesRegex(
             AssertionError, 'Cannot compute value on 2023-03-12 which is '
                             'before the issue date 2023-04-01'):
             IBond('04/2023', 25, InterestRates()).value(date(2023, 3, 12))
 
     def test_value(self):
         ib = IBond('01/2022', 1000)
+        self.assertEqual(1000, ib.value(date(2022, 1, 1)))
         self.assertEqual(1000, ib.value(date(2022, 2, 2)))
         self.assertEqual(1085.60, ib.value(date(2023, 4, 1)))
 
         ib = IBond('04/2018', 1000)
         self.assertEqual(1184.80, ib.value(date(2023, 4, 1)))
         self.assertEqual(1223.60, ib.value(date(2023, 10, 1)))
```

