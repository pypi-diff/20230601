# Comparing `tmp/imageswift-0.5.tar.gz` & `tmp/imageswift-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imageswift-0.5.tar", last modified: Thu Jun  1 19:26:11 2023, max compression
+gzip compressed data, was "dist\imageswift-0.6.tar", last modified: Thu Jun  1 19:55:38 2023, max compression
```

## Comparing `imageswift-0.5.tar` & `imageswift-0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 19:26:11.500598 imageswift-0.5/
--rw-rw-rw-   0        0        0      673 2023-06-01 19:26:11.500598 imageswift-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 19:26:11.500598 imageswift-0.5/imageswift/
--rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.5/imageswift/__init__.py
--rw-rw-rw-   0        0        0     3231 2023-05-22 21:28:14.809527 imageswift-0.5/imageswift/predicting.py
--rw-rw-rw-   0        0        0     5839 2023-06-01 19:21:08.092267 imageswift-0.5/imageswift/training.py
--rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.5/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-01 19:24:51.131193 imageswift-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:55:38.849095 imageswift-0.6/
+-rw-rw-rw-   0        0        0      673 2023-06-01 19:55:38.849095 imageswift-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 19:55:38.848094 imageswift-0.6/imageswift/
+-rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.6/imageswift/__init__.py
+-rw-rw-rw-   0        0        0     3231 2023-05-22 21:28:14.809527 imageswift-0.6/imageswift/predicting.py
+-rw-rw-rw-   0        0        0     5867 2023-06-01 19:51:04.948261 imageswift-0.6/imageswift/training.py
+-rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-01 19:52:54.204676 imageswift-0.6/setup.py
```

### Comparing `imageswift-0.5/PKG-INFO` & `imageswift-0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imageswift
-Version: 0.5
+Version: 0.6
 Summary: Easily train an image recognition model on your own images.
 Home-page: https://github.com/Suchisrit/ImageSwift
 Author: Suchisrit Gangopadhyay
 Author-email: suchisrit@gmail.com
 License: MIT
-Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.5.tar.gz
+Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.6.tar.gz
 Description: UNKNOWN
 Keywords: CV,Image Recognition,AI,ML
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imageswift-0.5/imageswift/predicting.py` & `imageswift-0.6/imageswift/predicting.py`

 * *Files identical despite different names*

### Comparing `imageswift-0.5/imageswift/training.py` & `imageswift-0.6/imageswift/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,16 @@
         ax.legend(loc = 1)    
         ax.set_ylim([0.01, 1])
 
         ax.set_xlabel(xlabel)
         ax.set_ylabel('Accuracy (Fraction)')
         
         plt.show()
-    def finishModel(self):
+    def trainModel(self):
+        self.loadDatasets()
         model = self.fnMakeModel()
 
         model.compile(
             optimizer=keras.optimizers.Adam(self.lr),
             loss=self.strLoss,
             metrics=["accuracy"],
         )
```

### Comparing `imageswift-0.5/setup.py` & `imageswift-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'imageswift',         
   packages = ['imageswift'],   
-  version = '0.5',      
+  version = '0.6',      
   license='MIT',        
   description = 'Easily train an image recognition model on your own images.',   
   author = 'Suchisrit Gangopadhyay',                  
   author_email = 'suchisrit@gmail.com',      
   url = 'https://github.com/Suchisrit/ImageSwift',   
-  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.5.tar.gz',  
+  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.6.tar.gz',  
   keywords = ['CV', 'Image Recognition', 'AI', 'ML'],   
   install_requires=[            
           'tensorflow==2.3.0',
           'seaborn==0.11.2',
           'pandas==1.2.0',
           'matplotlib==3.3.0'
       ],
```

