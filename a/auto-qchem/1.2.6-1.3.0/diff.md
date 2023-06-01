# Comparing `tmp/auto-qchem-1.2.6.tar.gz` & `tmp/auto-qchem-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-qchem-1.2.6.tar", last modified: Wed May 31 04:38:19 2023, max compression
+gzip compressed data, was "dist/auto-qchem-1.3.0.tar", last modified: Thu Jun  1 05:19:04 2023, max compression
```

## Comparing `auto-qchem-1.2.6.tar` & `auto-qchem-1.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/
--rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.2.6/LICENSE.md
--rw-r--r--   0 mac        (501) staff       (20)      283 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2334 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      283 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      593 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      199 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/auto_qchem.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/autoqchem/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/autoqchem/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    24645 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/autoqchem/db_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.2.6/autoqchem/descriptor_functions.py
--rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.2.6/autoqchem/draw_utils.py
--rw-r--r--   0 mac        (501) staff       (20)     6445 2023-05-30 21:03:35.000000 auto-qchem-1.2.6/autoqchem/gaussian_input_generator.py
--rw-r--r--   0 mac        (501) staff       (20)    19324 2023-05-30 23:48:03.000000 auto-qchem-1.2.6/autoqchem/gaussian_log_extractor.py
--rw-r--r--   0 mac        (501) staff       (20)     5086 2023-05-31 00:05:28.000000 auto-qchem-1.2.6/autoqchem/helper_classes.py
--rw-r--r--   0 mac        (501) staff       (20)     4234 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/autoqchem/helper_functions.py
--rw-r--r--   0 mac        (501) staff       (20)     2536 2023-05-30 22:10:02.000000 auto-qchem-1.2.6/autoqchem/molecule.py
--rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.2.6/autoqchem/openbabel_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    11206 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/autoqchem/rdkit_utils.py
--rw-r--r--   0 mac        (501) staff       (20)    28155 2023-05-25 06:48:01.000000 auto-qchem-1.2.6/autoqchem/sge_manager.py
--rw-r--r--   0 mac        (501) staff       (20)    25908 2023-05-25 06:46:41.000000 auto-qchem-1.2.6/autoqchem/slurm_manager.py
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-30 21:01:53.000000 auto-qchem-1.2.6/autoqchem/test.py
--rw-r--r--   0 mac        (501) staff       (20)      211 2023-05-25 06:45:53.000000 auto-qchem-1.2.6/config.yml
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-31 04:38:19.000000 auto-qchem-1.2.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      989 2023-05-31 04:37:12.000000 auto-qchem-1.2.6/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/
+-rw-r--r--   0 mac        (501) staff       (20)    35149 2022-10-06 20:25:51.000000 auto-qchem-1.3.0/LICENSE.md
+-rw-r--r--   0 mac        (501) staff       (20)      306 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1442 2023-05-31 05:41:29.000000 auto-qchem-1.3.0/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      306 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      593 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      221 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/auto_qchem.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/autoqchem/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-25 06:45:53.000000 auto-qchem-1.3.0/autoqchem/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    24645 2023-05-25 06:45:53.000000 auto-qchem-1.3.0/autoqchem/db_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2587 2022-10-06 20:25:51.000000 auto-qchem-1.3.0/autoqchem/descriptor_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)      981 2022-10-06 20:25:51.000000 auto-qchem-1.3.0/autoqchem/draw_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)     6445 2023-05-30 21:03:35.000000 auto-qchem-1.3.0/autoqchem/gaussian_input_generator.py
+-rw-r--r--   0 mac        (501) staff       (20)    19324 2023-05-30 23:48:03.000000 auto-qchem-1.3.0/autoqchem/gaussian_log_extractor.py
+-rw-r--r--   0 mac        (501) staff       (20)     5086 2023-05-31 00:05:28.000000 auto-qchem-1.3.0/autoqchem/helper_classes.py
+-rw-r--r--   0 mac        (501) staff       (20)     4234 2023-05-25 06:45:53.000000 auto-qchem-1.3.0/autoqchem/helper_functions.py
+-rw-r--r--   0 mac        (501) staff       (20)     2536 2023-05-30 22:10:02.000000 auto-qchem-1.3.0/autoqchem/molecule.py
+-rw-r--r--   0 mac        (501) staff       (20)     2274 2023-05-30 22:08:50.000000 auto-qchem-1.3.0/autoqchem/openbabel_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    11206 2023-05-25 06:45:53.000000 auto-qchem-1.3.0/autoqchem/rdkit_utils.py
+-rw-r--r--   0 mac        (501) staff       (20)    28155 2023-06-01 01:47:41.000000 auto-qchem-1.3.0/autoqchem/sge_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)    25908 2023-05-25 06:46:41.000000 auto-qchem-1.3.0/autoqchem/slurm_manager.py
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-30 21:01:53.000000 auto-qchem-1.3.0/autoqchem/test.py
+-rw-r--r--   0 mac        (501) staff       (20)      211 2023-05-25 06:45:53.000000 auto-qchem-1.3.0/config.yml
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-01 05:19:04.000000 auto-qchem-1.3.0/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1089 2023-06-01 05:18:45.000000 auto-qchem-1.3.0/setup.py
```

### Comparing `auto-qchem-1.2.6/LICENSE.md` & `auto-qchem-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/auto_qchem.egg-info/SOURCES.txt` & `auto-qchem-1.3.0/auto_qchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/db_functions.py` & `auto-qchem-1.3.0/autoqchem/db_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/descriptor_functions.py` & `auto-qchem-1.3.0/autoqchem/descriptor_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/draw_utils.py` & `auto-qchem-1.3.0/autoqchem/draw_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/gaussian_input_generator.py` & `auto-qchem-1.3.0/autoqchem/gaussian_input_generator.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/gaussian_log_extractor.py` & `auto-qchem-1.3.0/autoqchem/gaussian_log_extractor.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/helper_classes.py` & `auto-qchem-1.3.0/autoqchem/helper_classes.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/helper_functions.py` & `auto-qchem-1.3.0/autoqchem/helper_functions.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/molecule.py` & `auto-qchem-1.3.0/autoqchem/molecule.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/openbabel_utils.py` & `auto-qchem-1.3.0/autoqchem/openbabel_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/rdkit_utils.py` & `auto-qchem-1.3.0/autoqchem/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/autoqchem/sge_manager.py` & `auto-qchem-1.3.0/autoqchem/sge_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
             logger.warning(f"Job {job.base_name} failed  - could not retrieve log file. Cannot resubmit.")
 
         # clean up files on the remote site - do not cleanup anything, the /scratch/network cleans
         # up files that are older than 15 days
 
         return job.status
 
-    def resubmit_incomplete_jobs(self, wall_time="24:59:00") -> None:
+    def resubmit_incomplete_jobs(self, wall_time="23:59:00") -> None:
         """Resubmit jobs that are incomplete. If the job has failed because the optimization has not completed \
         and a log file has been retrieved, then \
         the last geometry will be used for the next submission. For failed jobs \
          the job input files will need to be fixed manually and submitted using the \
         function :py:meth:`~sge_manager.sge_manager.submit_jobs_from_jobs_dict`.\
          Maximum number of allowed submission of the same job is 3.
 
@@ -540,15 +540,15 @@
             ret = self.connection.run(f"qstat -u {self.user}", hide=True)
             #data = np.array(list(map(str.split, ret.stdout.splitlines())))
             if len(ret.stdout) > 0:
                 #return pd.DataFrame(data[1:], columns=data[0])
                 for l in ret.stdout.splitlines():
                     print(l)
             else: 
-                return "No jobs in queue"
+                print("No jobs in queue")
 
     def _qdel(self) -> None:
         """Run 'qdel -u $user' command on the server."""
 
         self.connect()
         self.connection.run(f"qdel -u {self.user}")
         self.remove_jobs(self.get_jobs(status=sge_status.submitted))
```

### Comparing `auto-qchem-1.2.6/autoqchem/slurm_manager.py` & `auto-qchem-1.3.0/autoqchem/slurm_manager.py`

 * *Files identical despite different names*

### Comparing `auto-qchem-1.2.6/setup.py` & `auto-qchem-1.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from setuptools import setup
 
 setup(
     name='auto-qchem',
-    version='1.2.6',
+    version='1.3.0',
     packages=['autoqchem'],
     data_files=['config.yml'],
     url='https://github.com/doyle-lab-ucla/auto-qchem',
     license='GPL',
     author='Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee',
     description='auto-qchem',
     long_description='automated dft calculation management software',
-    install_requires=['numpy==1.21',
-                      'pandas==1.3',
-                      'pyyaml==6.0',
-                      'scipy==1.7',
-                      'fabric==2.6',
-                      'paramiko==3.1',
-                      'pymongo==3.10',
-                      'appdirs==1.4',
-                      'ipywidgets==8.0',
-                      'py3Dmol==1.8',
+    install_requires=['numpy>=1.22',
+                      'pandas>=1.3',
+                      'pyyaml>=6.0',
+                      'scipy>=1.7',
+                      'fabric>=2.6',
+                      'paramiko>=3.1',
+                      'pymongo>=3.10',
+                      'appdirs>=1.4',
+                      'ipywidgets>=8.0',
+                      'py3Dmol>=1.8',
                       'jupyterlab>=3.4',
                       'notebook>=6.4',
                       'ipywidgets>=8.0',
                       'xlrd>=2.0',
                       'openpyxl>=3.0',
-                      ]
+                      'rdkit',
+                      'matplotlib>=3.5'
+                      ],
+    python_requires='>=3.8'
 )
```

