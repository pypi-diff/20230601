# Comparing `tmp/tupa123-1.5.3.tar.gz` & `tmp/tupa123-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.3.tar", last modified: Tue May 30 20:43:47 2023, max compression
+gzip compressed data, was "tupa123-1.5.4.tar", last modified: Thu Jun  1 12:57:45 2023, max compression
```

## Comparing `tupa123-1.5.3.tar` & `tupa123-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 20:43:47.158297 tupa123-1.5.3/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-05-30 20:43:47.158297 tupa123-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 20:43:47.158297 tupa123-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-05-30 20:40:37.000000 tupa123-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:43:47.148295 tupa123-1.5.3/tupa12/
--rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.3/tupa12/__init__.py
--rw-rw-rw-   0        0        0    50672 2023-05-30 19:47:13.000000 tupa123-1.5.3/tupa12/tupa12.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:43:47.148295 tupa123-1.5.3/tupa123/
--rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.3/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.3/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    89844 2023-05-29 20:11:26.000000 tupa123-1.5.3/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-05-30 20:43:47.158297 tupa123-1.5.3/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-05-30 20:43:46.000000 tupa123-1.5.3/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-30 20:43:47.000000 tupa123-1.5.3/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 20:43:46.000000 tupa123-1.5.3/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-30 20:43:46.000000 tupa123-1.5.3/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-30 20:43:46.000000 tupa123-1.5.3/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.382342 tupa123-1.5.4/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-06-01 12:57:45.382342 tupa123-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 12:57:45.382342 tupa123-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-01 12:57:20.000000 tupa123-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.351099 tupa123-1.5.4/tupa12/
+-rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.4/tupa12/__init__.py
+-rw-rw-rw-   0        0        0    50693 2023-06-01 12:55:36.000000 tupa123-1.5.4/tupa12/tupa12.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.366720 tupa123-1.5.4/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.4/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.4/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    89865 2023-06-01 12:55:39.000000 tupa123-1.5.4/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.366720 tupa123-1.5.4/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.3/LICENSE.txt` & `tupa123-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.3/PKG-INFO` & `tupa123-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.3
+Version: 1.5.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.3/README.md` & `tupa123-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.3/setup.py` & `tupa123-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.3',
+    version='1.5.4',
     license = 'MIT',
     license_files=('LICENSE.txt',),
     packages=['tupa123', 'tupa12'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
```

### Comparing `tupa123-1.5.3/tupa12/tupa12.py` & `tupa123-1.5.4/tupa12/tupa12.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 
 #Neural network 3 layers--------------------------------------------------------------------------------------------------------------------
 class nnet3:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.rate=rate
         self.epochs=epochs
         self.fa2c=fa2c
@@ -37,14 +37,15 @@
         self.shift=shift
         self.iteconv=iteconv
         self.conv=conv
         self.sbw=sbw
         self.c1=c1
         self.txt=txt
         self.sdnoise=sdnoise
+        self.c2=c2
 
 
 
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
@@ -241,15 +242,15 @@
             return y
 
         if (typee==16): # Metallic mean (inf,inf)
             y = (x + (x**2 + 4)**0.5)/2
             return y
 
         if (typee==17): #NoiseReLU (0,inf)            
-            y=np.where(x < 1e-8, 1e-8, x + np.random.normal(0,0.1) )
+            y=np.where(x < 0, 0, x * np.random.normal(1,self.c2) )
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
             y=np.where(x <= 0, x, x*x )
             return y
 
 
@@ -323,15 +324,15 @@
             return y
 
         if (typee==16): # Metallic mean (inf,inf)
             y = 0.5*((x/((x**2 + 4)**0.5))+1)            
             return y
 
         if (typee==17): #RandReLU (0,inf)
-            y=np.where(x < 1e-8, 1e-8, 1)
+            y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
             y=np.where(x <= 0, 1, 2*x )
             return y
         
 ###############################################################
```

### Comparing `tupa123-1.5.3/tupa123/machine1.txt` & `tupa123-1.5.4/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.3/tupa123/tupa123.py` & `tupa123-1.5.4/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -767,15 +767,15 @@
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
@@ -791,14 +791,15 @@
         self.shift=shift
         self.iteconv=iteconv
         self.conv=conv
         self.sbw=sbw
         self.c1=c1
         self.txt=txt
         self.sdnoise=sdnoise
+        self.c2=c2
 
 
 
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
@@ -995,15 +996,15 @@
             return y
 
         if (typee==16): # Metallic mean (inf,inf)
             y = (x + (x**2 + 4)**0.5)/2
             return y
 
         if (typee==17): #NoiseReLU (0,inf)            
-            y=np.where(x < 1e-8, 1e-8, x + np.random.normal(0,0.1) )
+            y=np.where(x < 0, 0, x * np.random.normal(1,self.c2) )
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
             y=np.where(x <= 0, x, x*x )
             return y
 
 
@@ -1077,15 +1078,15 @@
             return y
 
         if (typee==16): # Metallic mean (inf,inf)
             y = 0.5*((x/((x**2 + 4)**0.5))+1)            
             return y
 
         if (typee==17): #RandReLU (0,inf)
-            y=np.where(x < 1e-8, 1e-8, 1)
+            y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
             y=np.where(x <= 0, 1, 2*x )
             return y
         
 ###############################################################
```

### Comparing `tupa123-1.5.3/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.4/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.3
+Version: 1.5.4
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

