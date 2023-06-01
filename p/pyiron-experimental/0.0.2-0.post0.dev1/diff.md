# Comparing `tmp/pyiron_experimental-0.0.2.tar.gz` & `tmp/pyiron_experimental-0.post0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_experimental-0.0.2.tar", last modified: Tue Oct  5 05:17:08 2021, max compression
+gzip compressed data, was "pyiron_experimental-0.post0.dev1.tar", last modified: Thu Jun  1 14:35:15 2023, max compression
```

## Comparing `pyiron_experimental-0.0.2.tar` & `pyiron_experimental-0.post0.dev1.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       78 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/pyiron_experimental/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/pyiron_experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/pyiron_experimental/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2637 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/pyiron_experimental/matchseries.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/pyiron_experimental/pystemjob.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/pyiron_experimental/temmetajob.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      950 2021-10-05 05:17:08.000000 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      442 2021-10-05 05:17:08.000000 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-05 05:17:08.000000 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-05 05:17:08.000000 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-10-05 05:17:08.000000 pyiron_experimental-0.0.2/pyiron_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      207 2021-10-05 05:17:08.278473 pyiron_experimental-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2021-10-05 05:17:07.000000 pyiron_experimental-0.0.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68610 2021-10-05 05:17:04.000000 pyiron_experimental-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/pyiron_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/pyiron_experimental/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/image_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/matchseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/pystemjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/reload_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/resistance_mdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/run_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/tem_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental/temmetajob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 14:35:15.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 14:35:15.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:35:15.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 14:35:15.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 14:35:15.000000 pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-01 14:35:14.000000 pyiron_experimental-0.post0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:35:15.322450 pyiron_experimental-0.post0.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/tests/test_hs_line_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/tests/test_mdi_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68610 2023-06-01 14:35:11.000000 pyiron_experimental-0.post0.dev1/versioneer.py
```

### Comparing `pyiron_experimental-0.0.2/LICENSE` & `pyiron_experimental-0.post0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_experimental-0.0.2/PKG-INFO` & `pyiron_experimental-0.post0.dev1/pyiron_experimental.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
-Name: pyiron_experimental
-Version: 0.0.2
+Name: pyiron-experimental
+Version: 0.post0.dev1
 Summary: Repository for experimental plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_experimental
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: hassani@mpie.de
 License: BSD
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
 
 http://pyiron.org
-
```

### Comparing `pyiron_experimental-0.0.2/pyiron_experimental/matchseries.py` & `pyiron_experimental-0.post0.dev1/pyiron_experimental/matchseries.py`

 * *Files identical despite different names*

### Comparing `pyiron_experimental-0.0.2/pyiron_experimental/pystemjob.py` & `pyiron_experimental-0.post0.dev1/pyiron_experimental/pystemjob.py`

 * *Files identical despite different names*

### Comparing `pyiron_experimental-0.0.2/pyiron_experimental/temmetajob.py` & `pyiron_experimental-0.post0.dev1/pyiron_experimental/temmetajob.py`

 * *Files identical despite different names*

### Comparing `pyiron_experimental-0.0.2/pyiron_experimental.egg-info/PKG-INFO` & `pyiron_experimental-0.post0.dev1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
-Name: pyiron-experimental
-Version: 0.0.2
+Name: pyiron_experimental
+Version: 0.post0.dev1
 Summary: Repository for experimental plugins to the pyiron IDE.
 Home-page: https://github.com/pyiron/pyiron_experimental
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: hassani@mpie.de
 License: BSD
 Keywords: pyiron
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE
 
 http://pyiron.org
-
```

### Comparing `pyiron_experimental-0.0.2/setup.py` & `pyiron_experimental-0.post0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8'
     ],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*"]),
     install_requires=[
-        'pyiron_base>=0.3.5',
-        'matplotlib>=3.4.3',
+        'pyiron_base>=0.5.29',
+        'matplotlib>=3.6.2',
         'temmeta>=0.0.6',
         'pystem>=0.0.26',
-        'hyperspy>=1.6.4',
+        'hyperspy>=1.7.3',
         'scanf>=1.5.2',
     ],
     cmdclass=versioneer.get_cmdclass(),
 )
```

### Comparing `pyiron_experimental-0.0.2/versioneer.py` & `pyiron_experimental-0.post0.dev1/versioneer.py`

 * *Files identical despite different names*

