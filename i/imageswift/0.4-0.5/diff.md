# Comparing `tmp/imageswift-0.4.tar.gz` & `tmp/imageswift-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\imageswift-0.4.tar", last modified: Mon May 22 21:29:26 2023, max compression
+gzip compressed data, was "dist\imageswift-0.5.tar", last modified: Thu Jun  1 19:26:11 2023, max compression
```

## Comparing `imageswift-0.4.tar` & `imageswift-0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 21:29:26.268805 imageswift-0.4/
--rw-rw-rw-   0        0        0      673 2023-05-22 21:29:26.268805 imageswift-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 21:29:26.268805 imageswift-0.4/imageswift/
--rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.4/imageswift/__init__.py
--rw-rw-rw-   0        0        0     3231 2023-05-22 21:28:14.809527 imageswift-0.4/imageswift/predicting.py
--rw-rw-rw-   0        0        0     5805 2023-05-22 20:06:46.957769 imageswift-0.4/imageswift/training.py
--rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.4/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-05-22 21:29:21.730802 imageswift-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 19:26:11.500598 imageswift-0.5/
+-rw-rw-rw-   0        0        0      673 2023-06-01 19:26:11.500598 imageswift-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 19:26:11.500598 imageswift-0.5/imageswift/
+-rw-rw-rw-   0        0        0       90 2023-05-22 20:36:49.313731 imageswift-0.5/imageswift/__init__.py
+-rw-rw-rw-   0        0        0     3231 2023-05-22 21:28:14.809527 imageswift-0.5/imageswift/predicting.py
+-rw-rw-rw-   0        0        0     5839 2023-06-01 19:21:08.092267 imageswift-0.5/imageswift/training.py
+-rw-rw-rw-   0        0        0       40 2023-05-22 19:49:02.487025 imageswift-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-01 19:24:51.131193 imageswift-0.5/setup.py
```

### Comparing `imageswift-0.4/PKG-INFO` & `imageswift-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: imageswift
-Version: 0.4
+Version: 0.5
 Summary: Easily train an image recognition model on your own images.
 Home-page: https://github.com/Suchisrit/ImageSwift
 Author: Suchisrit Gangopadhyay
 Author-email: suchisrit@gmail.com
 License: MIT
-Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.4.tar.gz
+Download-URL: https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.5.tar.gz
 Description: UNKNOWN
 Keywords: CV,Image Recognition,AI,ML
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `imageswift-0.4/imageswift/predicting.py` & `imageswift-0.5/imageswift/predicting.py`

 * *Files identical despite different names*

### Comparing `imageswift-0.4/imageswift/training.py` & `imageswift-0.5/imageswift/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 import matplotlib.pyplot as plt
 
 from tensorflow.keras.models import Sequential
 from tensorflow.keras.applications import DenseNet201
 from tensorflow.keras.layers import Dropout, Dense, GlobalAveragePooling2D
 
 class ImageModel():
-    def __init__(self, strMainPath, strDataset, epochs=50, image_size=(150, 150), batch_size=32, validation_split=0.2):
+    def __init__(self, strMainPath, strDataset, epochs=50, image_size=(150, 150), batch_size=32, validation_split=0.2, lr=1e-3):
         self.strMainPath = strMainPath
         self.strDataset = strDataset
         self.strDatasetPath = os.path.join(self.strMainPath, self.strDataset)
         self.batch_size = batch_size
         self.image_size = image_size
         self.input_shape = self.image_size + (3,)
         self.lstClasses = os.listdir(self.strDatasetPath)
         self.num_classes = len(self.lstClasses)
         self.intEpochs = epochs
         self.val_split = validation_split
+        self.lr = lr
     def loadDatasets(self):
         train_ds = tf.keras.preprocessing.image_dataset_from_directory(
             self.strDatasetPath,
             validation_split=self.val_split,
             subset="training",
             seed=1337,
             image_size=self.image_size,
@@ -122,15 +123,15 @@
         ax.set_ylabel('Accuracy (Fraction)')
         
         plt.show()
     def finishModel(self):
         model = self.fnMakeModel()
 
         model.compile(
-            optimizer=keras.optimizers.Adam(1e-3),
+            optimizer=keras.optimizers.Adam(self.lr),
             loss=self.strLoss,
             metrics=["accuracy"],
         )
         history = model.fit(self.train_ds, epochs=self.intEpochs, validation_data=self.val_ds)
 
         self.plot_acc(history)
```

### Comparing `imageswift-0.4/setup.py` & `imageswift-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'imageswift',         
   packages = ['imageswift'],   
-  version = '0.4',      
+  version = '0.5',      
   license='MIT',        
   description = 'Easily train an image recognition model on your own images.',   
   author = 'Suchisrit Gangopadhyay',                  
   author_email = 'suchisrit@gmail.com',      
   url = 'https://github.com/Suchisrit/ImageSwift',   
-  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.4.tar.gz',  
+  download_url = 'https://github.com/Suchisrit/ImageSwift/archive/refs/tags/v0.5.tar.gz',  
   keywords = ['CV', 'Image Recognition', 'AI', 'ML'],   
   install_requires=[            
           'tensorflow==2.3.0',
           'seaborn==0.11.2',
           'pandas==1.2.0',
           'matplotlib==3.3.0'
       ],
```

