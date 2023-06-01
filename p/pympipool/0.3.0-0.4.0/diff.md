# Comparing `tmp/pympipool-0.3.0.tar.gz` & `tmp/pympipool-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.3.0.tar", last modified: Tue Mar 28 23:22:59 2023, max compression
+gzip compressed data, was "pympipool-0.4.0.tar", last modified: Thu Jun  1 19:00:01 2023, max compression
```

## Comparing `pympipool-0.3.0.tar` & `pympipool-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 23:22:59.633566 pympipool-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-03-28 23:22:56.000000 pympipool-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 23:22:56.000000 pympipool-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-28 23:22:59.633566 pympipool-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-28 23:22:56.000000 pympipool-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 23:22:59.633566 pympipool-0.3.0/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-03-28 23:22:56.000000 pympipool-0.3.0/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-28 23:22:56.000000 pympipool-0.3.0/pympipool/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-28 23:22:59.633566 pympipool-0.3.0/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 23:22:59.633566 pympipool-0.3.0/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-28 23:22:59.000000 pympipool-0.3.0/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-28 23:22:59.633566 pympipool-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-28 23:22:59.000000 pympipool-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 23:22:59.633566 pympipool-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-28 23:22:56.000000 pympipool-0.3.0/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-28 23:22:56.000000 pympipool-0.3.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-28 23:22:56.000000 pympipool-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-01 18:59:57.000000 pympipool-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 18:59:57.000000 pympipool-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-01 19:00:01.239016 pympipool-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-01 18:59:57.000000 pympipool-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.243016 pympipool-0.4.0/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-01 19:00:01.243016 pympipool-0.4.0/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/executor/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 18:59:57.000000 pympipool-0.4.0/pympipool/share/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 19:00:01.000000 pympipool-0.4.0/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-01 19:00:01.243016 pympipool-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 19:00:00.000000 pympipool-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:00:01.239016 pympipool-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_futurepool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 18:59:57.000000 pympipool-0.4.0/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-01 18:59:57.000000 pympipool-0.4.0/versioneer.py
```

### Comparing `pympipool-0.3.0/LICENSE` & `pympipool-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.3.0/PKG-INFO` & `pympipool-0.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1
-Name: pympipool
-Version: 0.3.0
-Summary: pympipool - scale functions over multiple compute nodes using mpi4py
-Home-page: https://github.com/jan-janssen/pympipool
-Author-email: jan.janssen@outlook.com
-License: BSD
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pympipool
+[![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
+
 Scale functions over multiple compute nodes using mpi4py
 
 ## Functionality
 ### Serial subtasks 
 Write a python test file like `pool.py`: 
 ```python
 import numpy as np
 from pympipool import Pool
 
 def calc(i):
     return np.array(i ** 2)
 
 with Pool(cores=2) as p:
-    print(p.map(function=calc, lst=[1, 2, 3, 4]))
+    print(p.map(fn=calc, iterables=[1, 2, 3, 4]))
 ```
 
 You can execute the python file `pool.py` in a serial python process: 
 ```
 python pool.py
 >>> [array(1), array(4), array(9), array(16)]
 ```
@@ -45,35 +30,71 @@
 ```python
 from pympipool import Pool
 
 def calc(i, comm):
     return i, comm.Get_size(), comm.Get_rank()
 
 with Pool(cores=4, cores_per_task=2) as p:
-    print(p.map(function=calc, lst=[1, 2, 3, 4]))
+    print(p.map(fn=calc, iterables=[1, 2, 3, 4]))
 ```
 
 Here the user-defined function `calc()` receives an additional input parameter `comm` which represents the 
 MPI communicator. It can be used just like any other `mpi4py.COMM` object. Here just the size `Get_size()` 
 and the rank `Get_rank()` are returned. 
 
+### Futures Interface
+In additions to the `map()` function `pympipool` also implements the `concurrent.futures` interface. As the 
+tasks are executed in a parallel subprocess using mpi4py, an additional call to the update function `update()` 
+is required. Example `submit.py`:  
+```python
+import numpy as np
+from time import sleep
+from pympipool import Pool
+
+def calc(i):
+    return np.array(i ** 2)
+
+with Pool(cores=2) as p:
+    futures = [p.submit(calc, i=i) for i in [1, 2, 3, 4]]
+    print([f.done() for f in futures])
+    sleep(1)
+    p.update()
+    print([f.result() for f in futures if f.done()])
+```
+After the submission using the submit function `submit()` the futures objects are not completed `done()`. Following,
+a short call of the sleep function the update function `update()` synchronizes the local futures objects. Consequently, 
+the future objects are afterward completed `done()` and the results can be received using the results function 
+`result()`. The code above results in the following output:
+```
+python submit.py
+>>> [False, False, False, False]
+>>> [array(1), array(4), array(9), array(16)]
+```
+
 ## Installation
 As `pympipool` requires `mpi` and `mpi4py` it is highly recommended to install it via conda: 
 ```
 conda install -c conda-forge pympipool
 ```
 Alternatively, it is also possible to `pympipool` via `pip`: 
 ```
 pip install pympipool
 ```
 
 ## Changelog
+### 0.4.0 
+* Update test coverage calculation.
+* Add `flux-framework` integration.
+* Change interface to be compatible to `concurrent.futures.Executor` - not backwards compatible.
+
 ### 0.3.0
 * Support subtasks with multiple MPI ranks. 
-* Close communication socket when closing the `pympipool.Pool`. 
+* Close communication socket when closing the `pympipool.Pool`.
+* `tqdm` compatibility is updated from `4.64.1` to `4.65.0`
+* `pyzmq` compatibility is updated from `25.0.0` to `25.0.2`
 
 ### 0.2.0
 * Communicate via zmq rather than `stdin` and `stdout`, this enables support for `mpich` and `openmpi`.
 * Add error handling to propagate the `Exception`, when it is raised by mapping the function to the arguments.
 
 ### 0.1.0
 * Major switch of the communication interface between the serial python process and the mpi parallel python process.
```

### Comparing `pympipool-0.3.0/pympipool.egg-info/PKG-INFO` & `pympipool-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.3.0
+Version: 0.4.0
 Summary: pympipool - scale functions over multiple compute nodes using mpi4py
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
@@ -13,28 +13,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pympipool
+[![Unittests](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml/badge.svg)](https://github.com/pyiron/pympipool/actions/workflows/unittest-openmpi.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pyiron/pympipool/badge.svg?branch=main)](https://coveralls.io/github/pyiron/pympipool?branch=main)
+
 Scale functions over multiple compute nodes using mpi4py
 
 ## Functionality
 ### Serial subtasks 
 Write a python test file like `pool.py`: 
 ```python
 import numpy as np
 from pympipool import Pool
 
 def calc(i):
     return np.array(i ** 2)
 
 with Pool(cores=2) as p:
-    print(p.map(function=calc, lst=[1, 2, 3, 4]))
+    print(p.map(fn=calc, iterables=[1, 2, 3, 4]))
 ```
 
 You can execute the python file `pool.py` in a serial python process: 
 ```
 python pool.py
 >>> [array(1), array(4), array(9), array(16)]
 ```
@@ -45,35 +48,71 @@
 ```python
 from pympipool import Pool
 
 def calc(i, comm):
     return i, comm.Get_size(), comm.Get_rank()
 
 with Pool(cores=4, cores_per_task=2) as p:
-    print(p.map(function=calc, lst=[1, 2, 3, 4]))
+    print(p.map(fn=calc, iterables=[1, 2, 3, 4]))
 ```
 
 Here the user-defined function `calc()` receives an additional input parameter `comm` which represents the 
 MPI communicator. It can be used just like any other `mpi4py.COMM` object. Here just the size `Get_size()` 
 and the rank `Get_rank()` are returned. 
 
+### Futures Interface
+In additions to the `map()` function `pympipool` also implements the `concurrent.futures` interface. As the 
+tasks are executed in a parallel subprocess using mpi4py, an additional call to the update function `update()` 
+is required. Example `submit.py`:  
+```python
+import numpy as np
+from time import sleep
+from pympipool import Pool
+
+def calc(i):
+    return np.array(i ** 2)
+
+with Pool(cores=2) as p:
+    futures = [p.submit(calc, i=i) for i in [1, 2, 3, 4]]
+    print([f.done() for f in futures])
+    sleep(1)
+    p.update()
+    print([f.result() for f in futures if f.done()])
+```
+After the submission using the submit function `submit()` the futures objects are not completed `done()`. Following,
+a short call of the sleep function the update function `update()` synchronizes the local futures objects. Consequently, 
+the future objects are afterward completed `done()` and the results can be received using the results function 
+`result()`. The code above results in the following output:
+```
+python submit.py
+>>> [False, False, False, False]
+>>> [array(1), array(4), array(9), array(16)]
+```
+
 ## Installation
 As `pympipool` requires `mpi` and `mpi4py` it is highly recommended to install it via conda: 
 ```
 conda install -c conda-forge pympipool
 ```
 Alternatively, it is also possible to `pympipool` via `pip`: 
 ```
 pip install pympipool
 ```
 
 ## Changelog
+### 0.4.0 
+* Update test coverage calculation.
+* Add `flux-framework` integration.
+* Change interface to be compatible to `concurrent.futures.Executor` - not backwards compatible.
+
 ### 0.3.0
 * Support subtasks with multiple MPI ranks. 
-* Close communication socket when closing the `pympipool.Pool`. 
+* Close communication socket when closing the `pympipool.Pool`.
+* `tqdm` compatibility is updated from `4.64.1` to `4.65.0`
+* `pyzmq` compatibility is updated from `25.0.0` to `25.0.2`
 
 ### 0.2.0
 * Communicate via zmq rather than `stdin` and `stdout`, this enables support for `mpich` and `openmpi`.
 * Add error handling to propagate the `Exception`, when it is raised by mapping the function to the arguments.
 
 ### 0.1.0
 * Major switch of the communication interface between the serial python process and the mpi parallel python process.
```

### Comparing `pympipool-0.3.0/setup.py` & `pympipool-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,17 +27,11 @@
         'Programming Language :: Python :: 3.11'
     ],
     packages=find_packages(exclude=["*tests*", "*.ci_support*"]),
     install_requires=[
         'cloudpickle>=2.2.1',
         'mpi4py>=3.1.4',
         'tqdm>=4.65.0',
-        'pyzmq>=25.0.2'
+        'pyzmq>=25.1.0'
     ],
     cmdclass=versioneer.get_cmdclass(),
-
-    entry_points={
-            "console_scripts": [
-                'pympipool=pympipool.__main__:main'
-            ]
-    }
 )
```

### Comparing `pympipool-0.3.0/tests/test_communicator_split.py` & `pympipool-0.4.0/tests/test_communicator_split.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,22 @@
         rank_new = comm.Get_rank()
     else:
         size_new = 0
         rank_new = 0
     return size, rank, size_new, rank_new, input_parameter
 
 
-class TestPool(unittest.TestCase):
+class TestCommunicator(unittest.TestCase):
     def test_pool_serial(self):
         with Pool(cores=2, cores_per_task=1) as p:
-            output = p.map(function=get_ranks, lst=[1, 2, 3])
+            output = p.map(fn=get_ranks, iterables=[1, 2, 3])
         self.assertEqual(output[0], (2, 1, 0, 0, 1))
         self.assertEqual(output[1], (2, 1, 0, 0, 2))
         self.assertEqual(output[2], (2, 1, 0, 0, 3))
 
     def test_pool_parallel(self):
         with Pool(cores=2, cores_per_task=2) as p:
-            output = p.map(function=get_ranks, lst=[1, 2, 3, 4])
+            output = p.map(fn=get_ranks, iterables=[1, 2, 3, 4])
         self.assertEqual(output[0][::2], (2, 2, 1))
         self.assertEqual(output[1][::2], (2, 2, 2))
         self.assertEqual(output[2][::2], (2, 2, 3))
         self.assertEqual(output[3][::2], (2, 2, 4))
```

### Comparing `pympipool-0.3.0/tests/test_pool.py` & `pympipool-0.4.0/tests/test_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,33 +18,43 @@
 def calc_error_type_error(i):
     raise TypeError("calc_error value error")
 
 
 class TestPool(unittest.TestCase):
     def test_pool_serial(self):
         with Pool(cores=1) as p:
-            output = p.map(function=calc, lst=[1, 2, 3, 4])
+            output = p.map(fn=calc, iterables=[1, 2, 3, 4])
         self.assertEqual(output[0], 1)
         self.assertEqual(output[1], 4)
         self.assertEqual(output[2], 9)
         self.assertEqual(output[3], 16)
 
     def test_pool_parallel(self):
         with Pool(cores=2) as p:
-            output = p.map(function=calc, lst=[1, 2, 3, 4])
+            output = p.map(fn=calc, iterables=[1, 2, 3, 4])
         self.assertEqual(output[0], 1)
         self.assertEqual(output[1], 4)
         self.assertEqual(output[2], 9)
         self.assertEqual(output[3], 16)
 
     def test_pool_none(self):
         with Pool(cores=2) as p:
-            output = p.map(function=calc_none, lst=[1, 2, 3, 4])
+            output = p.map(fn=calc_none, iterables=[1, 2, 3, 4])
         self.assertEqual(output, [None, None, None, None])
 
     def test_pool_error(self):
         with self.assertRaises(ValueError):
             with Pool(cores=2) as p:
-                p.map(function=calc_error_value_error, lst=[1, 2, 3, 4])
+                p.map(fn=calc_error_value_error, iterables=[1, 2, 3, 4])
         with self.assertRaises(TypeError):
             with Pool(cores=2) as p:
-                p.map(function=calc_error_type_error, lst=[1, 2, 3, 4])
+                p.map(fn=calc_error_type_error, iterables=[1, 2, 3, 4])
+
+    def test_shutdown(self):
+        p = Pool(cores=1)
+        output = p.map(fn=calc, iterables=[1, 2, 3, 4])
+        p.shutdown(wait=True)
+        p.shutdown(wait=False)
+        self.assertEqual(output[0], 1)
+        self.assertEqual(output[1], 4)
+        self.assertEqual(output[2], 9)
+        self.assertEqual(output[3], 16)
```

### Comparing `pympipool-0.3.0/versioneer.py` & `pympipool-0.4.0/versioneer.py`

 * *Files identical despite different names*

