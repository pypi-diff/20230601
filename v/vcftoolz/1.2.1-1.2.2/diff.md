# Comparing `tmp/vcftoolz-1.2.1.tar.gz` & `tmp/vcftoolz-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcftoolz-1.2.1.tar", last modified: Tue May  9 03:14:53 2023, max compression
+gzip compressed data, was "vcftoolz-1.2.2.tar", last modified: Thu Jun  1 05:38:38 2023, max compression
```

## Comparing `vcftoolz-1.2.1.tar` & `vcftoolz-1.2.2.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.914941 vcftoolz-1.2.1/
--rwxrwxrwx   0 chet      (1000) chet      (1000)      220 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/AUTHORS.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3327 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/CONTRIBUTING.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      891 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/HISTORY.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1556 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/LICENSE
--rwxrwxrwx   0 chet      (1000) chet      (1000)      244 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/MANIFEST.in
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3825 2023-05-09 03:14:53.915941 vcftoolz-1.2.1/PKG-INFO
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1954 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/README.rst
-drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.558073 vcftoolz-1.2.1/docs/
--rwxrwxrwx   0 chet      (1000) chet      (1000)     6770 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/Makefile
--rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/authors.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     9411 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/conf.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)       33 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/contributing.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/history.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      451 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/index.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      713 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/installation.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     6463 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/make.bat
--rwxrwxrwx   0 chet      (1000) chet      (1000)       27 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/readme.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)     8624 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/docs/usage.rst
--rwxrwxrwx   0 chet      (1000) chet      (1000)      159 2023-05-09 03:14:53.922938 vcftoolz-1.2.1/setup.cfg
--rwxrwxrwx   0 chet      (1000) chet      (1000)     1858 2023-05-09 03:11:12.000000 vcftoolz-1.2.1/setup.py
-drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.632073 vcftoolz-1.2.1/tests/
--rwxrwxrwx   0 chet      (1000) chet      (1000)       24 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/__init__.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)      299 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/test_cli.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3198 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/tests/test_vcftoolz.py
-drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.727075 vcftoolz-1.2.1/vcftoolz/
--rwxrwxrwx   0 chet      (1000) chet      (1000)      113 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/__init__.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    13994 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/cli.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    28430 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/vcf_call_parser.py
--rwxrwxrwx   0 chet      (1000) chet      (1000)    45814 2023-05-05 03:49:57.000000 vcftoolz-1.2.1/vcftoolz/vcftoolz.py
-drwxrwxrwx   0 chet      (1000) chet      (1000)        0 2023-05-09 03:14:53.889942 vcftoolz-1.2.1/vcftoolz.egg-info/
--rwxrwxrwx   0 chet      (1000) chet      (1000)     3825 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/PKG-INFO
--rwxrwxrwx   0 chet      (1000) chet      (1000)      625 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/SOURCES.txt
--rwxrwxrwx   0 chet      (1000) chet      (1000)        1 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/dependency_links.txt
--rwxrwxrwx   0 chet      (1000) chet      (1000)       48 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/entry_points.txt
--rwxrwxrwx   0 chet      (1000) chet      (1000)        1 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/not-zip-safe
--rwxrwxrwx   0 chet      (1000) chet      (1000)       57 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/requires.txt
--rwxrwxrwx   0 chet      (1000) chet      (1000)       16 2023-05-09 03:14:50.000000 vcftoolz-1.2.1/vcftoolz.egg-info/top_level.txt
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:38.065079 vcftoolz-1.2.2/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      220 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/AUTHORS.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3327 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/CONTRIBUTING.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1027 2023-06-01 05:26:46.000000 vcftoolz-1.2.2/HISTORY.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1556 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/LICENSE
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      244 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/MANIFEST.in
+-rw-r--r--   0 chet      (1000) chet      (1000)     3984 2023-06-01 05:38:38.067082 vcftoolz-1.2.2/PKG-INFO
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     1954 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/README.rst
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.520564 vcftoolz-1.2.2/docs/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6770 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/Makefile
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/authors.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     9411 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/conf.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       33 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/contributing.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       28 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/history.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      451 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/index.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      713 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/installation.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     6463 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/make.bat
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       27 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/readme.rst
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     8624 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/docs/usage.rst
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.603562 vcftoolz-1.2.2/pyvenn/
+-rw-r--r--   0 chet      (1000) chet      (1000)        0 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/__init__.py
+-rw-r--r--   0 chet      (1000) chet      (1000)     1184 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/demo.py
+-rw-r--r--   0 chet      (1000) chet      (1000)    22120 2023-06-01 04:52:05.000000 vcftoolz-1.2.2/pyvenn/venn.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      159 2023-06-01 05:38:38.075079 vcftoolz-1.2.2/setup.cfg
+-rwxr-xr-x   0 chet      (1000) chet      (1000)     1887 2023-06-01 05:11:11.000000 vcftoolz-1.2.2/setup.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.691563 vcftoolz-1.2.2/tests/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)       24 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      299 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/test_cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)     3198 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/tests/test_vcftoolz.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:37.811081 vcftoolz-1.2.2/vcftoolz/
+-rwxrwxrwx   0 chet      (1000) chet      (1000)      113 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/__init__.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    13994 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/cli.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    28430 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/vcf_call_parser.py
+-rwxrwxrwx   0 chet      (1000) chet      (1000)    45814 2023-05-05 03:49:57.000000 vcftoolz-1.2.2/vcftoolz/vcftoolz.py
+drwxr-xr-x   0 chet      (1000) chet      (1000)        0 2023-06-01 05:38:38.033082 vcftoolz-1.2.2/vcftoolz.egg-info/
+-rw-r--r--   0 chet      (1000) chet      (1000)     3984 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/PKG-INFO
+-rw-r--r--   0 chet      (1000) chet      (1000)      674 2023-06-01 05:38:37.000000 vcftoolz-1.2.2/vcftoolz.egg-info/SOURCES.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/dependency_links.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)       48 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/entry_points.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)        1 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/not-zip-safe
+-rw-r--r--   0 chet      (1000) chet      (1000)       57 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/requires.txt
+-rw-r--r--   0 chet      (1000) chet      (1000)       16 2023-06-01 05:38:36.000000 vcftoolz-1.2.2/vcftoolz.egg-info/top_level.txt
```

### Comparing `vcftoolz-1.2.1/CONTRIBUTING.rst` & `vcftoolz-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/HISTORY.rst` & `vcftoolz-1.2.2/HISTORY.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 .. :changelog:
 
 History
 =======
 
+1.2.2 (2023-06-01)
+------------------
+* Fixed broken Pyvenn dependency
+
+1.2.1 (2023-05-09)
+------------------
+* Update PyVCF to PyVCF3
+
 1.2.0 (2019-04-04)
 ---------------------
 * Fix defect in narrow command wrongly printing ALT=. when GT=.
 * Add the ``count`` command to count samples, positions, calls, snps, indels,
   other variants, filtered calls, missing calls, and filter reasons.
 * Add the ``plot`` command to plot calls along the length of the genome and show
   the location of filtered calls.
```

### Comparing `vcftoolz-1.2.1/LICENSE` & `vcftoolz-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/PKG-INFO` & `vcftoolz-1.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
 Keywords: bioinformatics,NGS,vcftoolz
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 VCF Toolz
 ===============================
 
@@ -82,14 +83,22 @@
 
 
 
 
 History
 =======
 
+1.2.2 (2023-06-01)
+------------------
+* Fixed broken Pyvenn dependency
+
+1.2.1 (2023-05-09)
+------------------
+* Update PyVCF to PyVCF3
+
 1.2.0 (2019-04-04)
 ---------------------
 * Fix defect in narrow command wrongly printing ALT=. when GT=.
 * Add the ``count`` command to count samples, positions, calls, snps, indels,
   other variants, filtered calls, missing calls, and filter reasons.
 * Add the ``plot`` command to plot calls along the length of the genome and show
   the location of filtered calls.
```

### Comparing `vcftoolz-1.2.1/README.rst` & `vcftoolz-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/docs/Makefile` & `vcftoolz-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/docs/conf.py` & `vcftoolz-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/docs/installation.rst` & `vcftoolz-1.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/docs/make.bat` & `vcftoolz-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/docs/usage.rst` & `vcftoolz-1.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/setup.py` & `vcftoolz-1.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 test_requirements = [
     "pytest",
 ]
 
 setup(
     name='vcftoolz',
-    version='1.2.1',
+    version='1.2.2',
     description="Tools for working with Variant Call Format files.",
     long_description=readme + '\n\n' + history,
     author="Steve Davis",
     author_email='steven.davis@fda.hhs.gov',
     url='https://github.com/CFSAN-Biostatistics/vcftoolz',
     packages=[
         'pyvenn',
@@ -59,9 +59,10 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
     ],
     entry_points={'console_scripts': ['vcftoolz = vcftoolz.cli:main']},
     setup_requires=["pytest-runner"],
-    tests_require=test_requirements
+    tests_require=test_requirements,
+    python_requires=">=3.9"
 )
```

### Comparing `vcftoolz-1.2.1/tests/test_vcftoolz.py` & `vcftoolz-1.2.2/tests/test_vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/vcftoolz/cli.py` & `vcftoolz-1.2.2/vcftoolz/cli.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/vcftoolz/vcf_call_parser.py` & `vcftoolz-1.2.2/vcftoolz/vcf_call_parser.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/vcftoolz/vcftoolz.py` & `vcftoolz-1.2.2/vcftoolz/vcftoolz.py`

 * *Files identical despite different names*

### Comparing `vcftoolz-1.2.1/vcftoolz.egg-info/PKG-INFO` & `vcftoolz-1.2.2/vcftoolz.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcftoolz
-Version: 1.2.1
+Version: 1.2.2
 Summary: Tools for working with Variant Call Format files.
 Home-page: https://github.com/CFSAN-Biostatistics/vcftoolz
 Author: Steve Davis
 Author-email: steven.davis@fda.hhs.gov
 License: BSD
 Keywords: bioinformatics,NGS,vcftoolz
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ===============================
 VCF Toolz
 ===============================
 
@@ -82,14 +83,22 @@
 
 
 
 
 History
 =======
 
+1.2.2 (2023-06-01)
+------------------
+* Fixed broken Pyvenn dependency
+
+1.2.1 (2023-05-09)
+------------------
+* Update PyVCF to PyVCF3
+
 1.2.0 (2019-04-04)
 ---------------------
 * Fix defect in narrow command wrongly printing ALT=. when GT=.
 * Add the ``count`` command to count samples, positions, calls, snps, indels,
   other variants, filtered calls, missing calls, and filter reasons.
 * Add the ``plot`` command to plot calls along the length of the genome and show
   the location of filtered calls.
```

### Comparing `vcftoolz-1.2.1/vcftoolz.egg-info/SOURCES.txt` & `vcftoolz-1.2.2/vcftoolz.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
+pyvenn/__init__.py
+pyvenn/demo.py
+pyvenn/venn.py
 tests/__init__.py
 tests/test_cli.py
 tests/test_vcftoolz.py
 vcftoolz/__init__.py
 vcftoolz/cli.py
 vcftoolz/vcf_call_parser.py
 vcftoolz/vcftoolz.py
```

