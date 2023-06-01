# Comparing `tmp/clonalEvolution-2.1.0.tar.gz` & `tmp/clonalEvolution-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.1.0.tar", last modified: Thu Jun  1 06:44:14 2023, max compression
+gzip compressed data, was "clonalEvolution-2.1.1.tar", last modified: Thu Jun  1 06:46:07 2023, max compression
```

## Comparing `clonalEvolution-2.1.0.tar` & `clonalEvolution-2.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 06:44:14.250369 clonalEvolution-2.1.0/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-06-01 06:44:14.251366 clonalEvolution-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.1.0/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-06-01 06:44:14.252364 clonalEvolution-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-06-01 06:41:32.000000 clonalEvolution-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:44:14.198325 clonalEvolution-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 06:44:14.233414 clonalEvolution-2.1.0/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.1.0/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21476 2023-06-01 06:43:40.000000 clonalEvolution-2.1.0/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    25168 2023-06-01 06:41:59.000000 clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32641 2023-05-25 22:44:36.000000 clonalEvolution-2.1.0/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-25 22:36:13.000000 clonalEvolution-2.1.0/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.1.0/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:44:14.246380 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-01 06:44:14.000000 clonalEvolution-2.1.0/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 06:44:14.248374 clonalEvolution-2.1.0/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.1.0/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:46:07.255800 clonalEvolution-2.1.1/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-06-01 06:46:07.256798 clonalEvolution-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.1.1/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-06-01 06:46:07.257795 clonalEvolution-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-06-01 06:45:29.000000 clonalEvolution-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:46:07.211395 clonalEvolution-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 06:46:07.239842 clonalEvolution-2.1.1/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.1.1/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21476 2023-06-01 06:43:40.000000 clonalEvolution-2.1.1/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    25176 2023-06-01 06:45:48.000000 clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32641 2023-05-25 22:44:36.000000 clonalEvolution-2.1.1/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-25 22:36:13.000000 clonalEvolution-2.1.1/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.1.1/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:46:07.251848 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-01 06:46:07.000000 clonalEvolution-2.1.1/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 06:46:07.253806 clonalEvolution-2.1.1/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.1.1/tests/test_simple.py
```

### Comparing `clonalEvolution-2.1.0/LICENSE` & `clonalEvolution-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/PKG-INFO` & `clonalEvolution-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.1.0
+Version: 2.1.1
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.1.0/README.md` & `clonalEvolution-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/setup.py` & `clonalEvolution-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.1.0",
+    version="2.1.1",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/__main__.py` & `clonalEvolution-2.1.1/src/clonalEvolution/__main__.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
                 'Clone fitness': copy.deepcopy([row[5].tolist() for row in iPop]),
                 'Previous clone number': copy.deepcopy([row[6] for row in iPop])
             })
             tsf = Thread(target=saveMatrixData, args=(df, file_localization, file_name + '_matrix', copy.copy(iter_outer)))
             # saveMatrixData(df, file_localization, file_name + '_matrix', copy.copy(iter_outer))
             tsf.start()
 
-def clonalEvolutionMainLoop(iPop, params, file_name="", file_description="", file_localization="", plots=0, t_iter=-1, q=None, ID=0, select=0, end=10):
+def clonalEvolutionMainLoop(iPop, params, file_name="", file_description="", file_localization="", plots=0, t_iter=-1, q=None, ID=0, select=0, end_p=10):
     """
     Main simulation loop
         iPop: population array where row is in form of: 
             SINGLE CELL ALGORITH
                 Mutation number  
                 Fitness
                 Clone number
@@ -514,21 +514,21 @@
                 FILE.close()
             tx = time.time()
                 
         if (iter_outer % steps == 0 and iter_outer > 0):
             print('simulation ended, ID: %i' % ID)
             break
         if select == 0: 
-            if(len(iPop)) >= end*pop:
+            if(len(iPop)) >= end_p*pop:
                 break
         elif select == 1:
-            if(sum([row[1] for row in iPop])) >= end*pop:
+            if(sum([row[1] for row in iPop])) >= end_p*pop:
                 break
         elif select == 2:
-            if(sum([row[1] for row in iPop])) >= end*pop:
+            if(sum([row[1] for row in iPop])) >= end_p*pop:
                 break
         
         if select == 0:            
             iPop = CEL.clonalEvolutionLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads)
         elif select == 1:
             iPop = CEBL.clonalEvolutionBinnedLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
         elif select == 2:
```

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.1.1/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.1.1/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution/mainView.py` & `clonalEvolution-2.1.1/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.1.1/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.1.0
+Version: 2.1.1
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.1.0/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.1.1/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

