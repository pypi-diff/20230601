# Comparing `tmp/tupa123-1.5.4.tar.gz` & `tmp/tupa123-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.4.tar", last modified: Thu Jun  1 12:57:45 2023, max compression
+gzip compressed data, was "tupa123-1.5.5.tar", last modified: Thu Jun  1 18:58:01 2023, max compression
```

## Comparing `tupa123-1.5.4.tar` & `tupa123-1.5.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.382342 tupa123-1.5.4/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-06-01 12:57:45.382342 tupa123-1.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 12:57:45.382342 tupa123-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-01 12:57:20.000000 tupa123-1.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.351099 tupa123-1.5.4/tupa12/
--rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.4/tupa12/__init__.py
--rw-rw-rw-   0        0        0    50693 2023-06-01 12:55:36.000000 tupa123-1.5.4/tupa12/tupa12.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.366720 tupa123-1.5.4/tupa123/
--rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.4/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.4/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    89865 2023-06-01 12:55:39.000000 tupa123-1.5.4/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-06-01 12:57:45.366720 tupa123-1.5.4/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 12:57:45.000000 tupa123-1.5.4/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.871468 tupa123-1.5.5/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-06-01 18:58:01.870604 tupa123-1.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:58:01.871468 tupa123-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-01 18:57:23.000000 tupa123-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.850541 tupa123-1.5.5/tupa12/
+-rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.5/tupa12/__init__.py
+-rw-rw-rw-   0        0        0    50693 2023-06-01 18:56:11.000000 tupa123-1.5.5/tupa12/tupa12.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.858125 tupa123-1.5.5/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.5/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.5/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    89863 2023-06-01 18:56:09.000000 tupa123-1.5.5/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:58:01.868579 tupa123-1.5.5/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 18:58:01.000000 tupa123-1.5.5/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.4/LICENSE.txt` & `tupa123-1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.4/PKG-INFO` & `tupa123-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.4
+Version: 1.5.5
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.4/README.md` & `tupa123-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.4/setup.py` & `tupa123-1.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.4',
+    version='1.5.5',
     license = 'MIT',
     license_files=('LICENSE.txt',),
     packages=['tupa123', 'tupa12'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
```

### Comparing `tupa123-1.5.4/tupa12/tupa12.py` & `tupa123-1.5.5/tupa12/tupa12.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 
 #Neural network 3 layers--------------------------------------------------------------------------------------------------------------------
 class nnet3:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.rate=rate
         self.epochs=epochs
         self.fa2c=fa2c
@@ -38,14 +38,15 @@
         self.iteconv=iteconv
         self.conv=conv
         self.sbw=sbw
         self.c1=c1
         self.txt=txt
         self.sdnoise=sdnoise
         self.c2=c2
+        self.c3=c3
 
 
 
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
@@ -188,16 +189,15 @@
             y = np.log(1+np.exp(x)) #log é na base natural
             return y
 
         if (typee==3): #gaussinana (0,1)
             y = np.exp(-1*(x**2)) 
             return y
 
-        if (typee==4): #ReLU (0,inf)
-            #y=np.where(x < 1e-8, 1e-8, x)
+        if (typee==4): #ReLU (0,inf)            
             y=np.where(x < 0, 0, x)
             return y
 
         if (typee==5): #tanh (-1,1)
             y = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             return y
 
@@ -246,15 +246,15 @@
             return y
 
         if (typee==17): #NoiseReLU (0,inf)            
             y=np.where(x < 0, 0, x * np.random.normal(1,self.c2) )
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
-            y=np.where(x <= 0, x, x*x )
+            y=np.where(x < 0, 0, abs(x)**self.c3)
             return y
 
 
     def DeActivation(self, typee,x):
 
         if (typee==0): #linear (-inf,inf)
             y = 1
@@ -269,16 +269,15 @@
             y = 1/(1 + np.exp(-x))
             return y
     
         if (typee==3): #gaussinana (0,1)
             y = -2*x*np.exp(-1*(x**2)) 
             return y
 
-        if (typee==4): #ReLU (0,inf)
-            #y=np.where(x < 1e-8, 1e-8, 1)
+        if (typee==4): #ReLU (0,inf)            
             y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==5): #tanh (-1,1)
             w = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             y = 1 - w**2
             return y
@@ -328,15 +327,15 @@
             return y
 
         if (typee==17): #RandReLU (0,inf)
             y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
-            y=np.where(x <= 0, 1, 2*x )
+            y=np.where(x < 0, 0, self.c3*(abs(x)**(self.c3-1)) )
             return y
         
 ###############################################################
 ###############################################################
 ################ Machine learning   ###########################
 ###############################################################
 ###############################################################
```

### Comparing `tupa123-1.5.4/tupa123/machine1.txt` & `tupa123-1.5.5/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.4/tupa123/tupa123.py` & `tupa123-1.5.5/tupa123/tupa123.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,15 +767,15 @@
 
 
 
 #Neural network 4 layers--------------------------------------------------------------------------------------------------------------------
 class nnet4:
 
     #global variables-------------------------------------------------------------------------
-    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01):
+    def __init__ (self, norma=1, coef=0, normout=1, nn1c=1, nn2c=5, nn3c=5, nn4c=1, rate=0.01, epochs=1000, fa2c=5, fa3c=5, fa4c=0, cost=0, regu=0, namenet='', shift=1, iteconv=0, conv=0, sbw=1, c1=2, txt=0, sdnoise=0, c2=0.01, c3=1.33):
         
         self.nn1c=nn1c
         self.nn2c=nn2c
         self.nn3c=nn3c
         self.nn4c=nn4c
         self.rate=rate
         self.epochs=epochs
@@ -792,14 +792,15 @@
         self.iteconv=iteconv
         self.conv=conv
         self.sbw=sbw
         self.c1=c1
         self.txt=txt
         self.sdnoise=sdnoise
         self.c2=c2
+        self.c3=c3
 
 
 
 ###############################################################
 ###############################################################
 #########  Auxliar function to normalization   ################
 ###############################################################
@@ -942,16 +943,15 @@
             y = np.log(1+np.exp(x)) #log é na base natural
             return y
 
         if (typee==3): #gaussinana (0,1)
             y = np.exp(-1*(x**2)) 
             return y
 
-        if (typee==4): #ReLU (0,inf)
-            #y=np.where(x < 1e-8, 1e-8, x)
+        if (typee==4): #ReLU (0,inf)           
             y=np.where(x < 0, 0, x)
             return y
 
         if (typee==5): #tanh (-1,1)
             y = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             return y
 
@@ -1000,15 +1000,15 @@
             return y
 
         if (typee==17): #NoiseReLU (0,inf)            
             y=np.where(x < 0, 0, x * np.random.normal(1,self.c2) )
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
-            y=np.where(x <= 0, x, x*x )
+            y=np.where(x < 0, 0, abs(x)**self.c3)
             return y
 
 
     def DeActivation(self, typee,x):
 
         if (typee==0): #linear (-inf,inf)
             y = 1
@@ -1023,16 +1023,15 @@
             y = 1/(1 + np.exp(-x))
             return y
     
         if (typee==3): #gaussinana (0,1)
             y = -2*x*np.exp(-1*(x**2)) 
             return y
 
-        if (typee==4): #ReLU (0,inf)
-            #y=np.where(x < 1e-8, 1e-8, 1)
+        if (typee==4): #ReLU (0,inf)           
             y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==5): #tanh (-1,1)
             w = (np.exp(x)-np.exp(-x))/(np.exp(x)+np.exp(-x))
             y = 1 - w**2
             return y
@@ -1082,15 +1081,15 @@
             return y
 
         if (typee==17): #RandReLU (0,inf)
             y=np.where(x < 0, 0, 1)
             return y
 
         if (typee==18): #ReLUquad (-inf,inf)            
-            y=np.where(x <= 0, 1, 2*x )
+            y=np.where(x < 0, 0, self.c3*(abs(x)**(self.c3-1)) )
             return y
         
 ###############################################################
 ###############################################################
 ################ Machine learning   ###########################
 ###############################################################
 ###############################################################
```

### Comparing `tupa123-1.5.4/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.5/tupa123.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.4
+Version: 1.5.5
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

