# Comparing `tmp/Sigmoidal-0.2.1.tar.gz` & `tmp/Sigmoidal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sigmoidal-0.2.1.tar", last modified: Tue May 23 02:40:00 2023, max compression
+gzip compressed data, was "Sigmoidal-0.3.0.tar", last modified: Thu Jun  1 18:46:45 2023, max compression
```

## Comparing `Sigmoidal-0.2.1.tar` & `Sigmoidal-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-23 02:40:00.739531 Sigmoidal-0.2.1/
--rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 Sigmoidal-0.2.1/LICENSE
--rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 Sigmoidal-0.2.1/MANIFEST.in
--rw-r--r--   0 jade       (502) staff       (20)     1526 2023-05-23 02:40:00.739058 Sigmoidal-0.2.1/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)     1041 2023-05-22 21:50:35.000000 Sigmoidal-0.2.1/README.md
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-23 02:40:00.738577 Sigmoidal-0.2.1/Sigmoidal.egg-info/
--rw-r--r--   0 jade       (502) staff       (20)     1526 2023-05-23 02:40:00.000000 Sigmoidal-0.2.1/Sigmoidal.egg-info/PKG-INFO
--rw-r--r--   0 jade       (502) staff       (20)      388 2023-05-23 02:40:00.000000 Sigmoidal-0.2.1/Sigmoidal.egg-info/SOURCES.txt
--rw-r--r--   0 jade       (502) staff       (20)        1 2023-05-23 02:40:00.000000 Sigmoidal-0.2.1/Sigmoidal.egg-info/dependency_links.txt
--rw-r--r--   0 jade       (502) staff       (20)       28 2023-05-23 02:40:00.000000 Sigmoidal-0.2.1/Sigmoidal.egg-info/requires.txt
--rw-r--r--   0 jade       (502) staff       (20)       10 2023-05-23 02:40:00.000000 Sigmoidal-0.2.1/Sigmoidal.egg-info/top_level.txt
--rw-r--r--   0 jade       (502) staff       (20)       38 2023-05-23 02:40:00.739563 Sigmoidal-0.2.1/setup.cfg
--rw-r--r--   0 jade       (502) staff       (20)      723 2023-05-23 02:39:58.000000 Sigmoidal-0.2.1/setup.py
-drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-05-23 02:40:00.738677 Sigmoidal-0.2.1/sigmoidal/
--rw-r--r--   0 jade       (502) staff       (20)     4183 2023-05-22 21:14:28.000000 Sigmoidal-0.2.1/sigmoidal/__init__.py
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.887342 Sigmoidal-0.3.0/
+-rw-r--r--   0 jade       (502) staff       (20)     1063 2023-05-22 21:09:43.000000 Sigmoidal-0.3.0/LICENSE
+-rw-r--r--   0 jade       (502) staff       (20)        0 2023-05-22 21:14:28.000000 Sigmoidal-0.3.0/MANIFEST.in
+-rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-01 18:46:45.886799 Sigmoidal-0.3.0/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)     1057 2023-05-23 02:43:17.000000 Sigmoidal-0.3.0/README.md
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.886232 Sigmoidal-0.3.0/Sigmoidal.egg-info/
+-rw-r--r--   0 jade       (502) staff       (20)     1542 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/PKG-INFO
+-rw-r--r--   0 jade       (502) staff       (20)      388 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/SOURCES.txt
+-rw-r--r--   0 jade       (502) staff       (20)        1 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/dependency_links.txt
+-rw-r--r--   0 jade       (502) staff       (20)       28 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/requires.txt
+-rw-r--r--   0 jade       (502) staff       (20)       10 2023-06-01 18:46:45.000000 Sigmoidal-0.3.0/Sigmoidal.egg-info/top_level.txt
+-rw-r--r--   0 jade       (502) staff       (20)       38 2023-06-01 18:46:45.887377 Sigmoidal-0.3.0/setup.cfg
+-rw-r--r--   0 jade       (502) staff       (20)      723 2023-06-01 18:10:41.000000 Sigmoidal-0.3.0/setup.py
+drwxr-xr-x   0 jade       (502) staff       (20)        0 2023-06-01 18:46:45.886333 Sigmoidal-0.3.0/sigmoidal/
+-rw-r--r--   0 jade       (502) staff       (20)     4993 2023-06-01 18:46:08.000000 Sigmoidal-0.3.0/sigmoidal/__init__.py
```

### Comparing `Sigmoidal-0.2.1/LICENSE` & `Sigmoidal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Sigmoidal-0.2.1/PKG-INFO` & `Sigmoidal-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sigmoidal
-Version: 0.2.1
+Version: 0.3.0
 Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
 Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -28,8 +28,8 @@
 ## Setup for Deployment
 * `pip install twine`
 
 ## Building the Package
 * `python setup.py sdist bdist_wheel`
 
 ## Deploying
-* `twine upload --repository-url https://upload.pypi.org/legacy/ dist/*`
+* `twine upload --skip-existing --repository-url https://upload.pypi.org/legacy/ dist/*`
```

### Comparing `Sigmoidal-0.2.1/README.md` & `Sigmoidal-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 ## Setup for Deployment
 * `pip install twine`
 
 ## Building the Package
 * `python setup.py sdist bdist_wheel`
 
 ## Deploying
-* `twine upload --repository-url https://upload.pypi.org/legacy/ dist/*`
+* `twine upload --skip-existing --repository-url https://upload.pypi.org/legacy/ dist/*`
```

### Comparing `Sigmoidal-0.2.1/Sigmoidal.egg-info/PKG-INFO` & `Sigmoidal-0.3.0/Sigmoidal.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Sigmoidal
-Version: 0.2.1
+Version: 0.3.0
 Summary: Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.
 Home-page: https://github.com/HelloSleuth/sigmoid
 Author: Jade Glaze, Sleuth
 Author-email: jade@hellosleuth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -28,8 +28,8 @@
 ## Setup for Deployment
 * `pip install twine`
 
 ## Building the Package
 * `python setup.py sdist bdist_wheel`
 
 ## Deploying
-* `twine upload --repository-url https://upload.pypi.org/legacy/ dist/*`
+* `twine upload --skip-existing --repository-url https://upload.pypi.org/legacy/ dist/*`
```

### Comparing `Sigmoidal-0.2.1/setup.py` & `Sigmoidal-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Sigmoidal',
-    version='0.2.1',
+    version='0.3.0',
     author='Jade Glaze, Sleuth',
     author_email='jade@hellosleuth.com',
     url='https://github.com/HelloSleuth/sigmoid',
     license='MIT',
     description='Sigmoidal is a small library to allow you to fit and evaluate sigmoid functions in a way that works like the Numpy Polynomial class.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `Sigmoidal-0.2.1/sigmoidal/__init__.py` & `Sigmoidal-0.3.0/sigmoidal/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,16 +91,42 @@
             B = -math.log(-(b+L)/b)
             x = complex(x0+(B/k), 1)  # imaginary part is irrelevant but would be -(2*pi*n)/k for any integer n
             return x.real
         except (ZeroDivisionError, ValueError):  # ZeroDivision is obvious, ValueError is from log(0)
             return None  # no root
 
     @staticmethod
+    def _positive_scaled_sigmoid(x, L):
+        return L / (1 + np.exp(-x))
+
+    @staticmethod
+    def _negative_scaled_sigmoid(x, L):
+        e_ = np.exp(x)
+        return (L * e_) / (1 + e_)
+
+    @staticmethod
     def _sigmoid(x, L, x0, k, b):
-        y = L / (1 + np.exp(-k*(x-x0))) + b
+        x_ = k * (x - x0)
+
+        if isinstance(x_, np.ndarray):
+            positive_mask = x_ >= 0
+            negative_mask = ~positive_mask
+
+            y = np.empty_like(x_, dtype=np.float64)
+            y[positive_mask] = Sigmoid._positive_scaled_sigmoid(x_[positive_mask], L)
+            y[negative_mask] = Sigmoid._negative_scaled_sigmoid(x_[negative_mask], L)
+        else:
+            if x_ >= 0:
+                y = Sigmoid._positive_scaled_sigmoid(x_, L)
+            else:
+                y = Sigmoid._negative_scaled_sigmoid(x_, L)
+        y = y + b
+
+        # naive implementation
+        # y = L / (1 + np.exp(-k*(x-x0))) + b
         return y
 
     @staticmethod
     def _derivative_1(x, L, x0, k, *args):
         e_ = np.exp(-k*(x-x0))
         y = (k*L*e_)/((1+e_)**2)
         return y
```

