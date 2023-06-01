# Comparing `tmp/FeatureInsight-0.0.8.tar.gz` & `tmp/FeatureInsight-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FeatureInsight-0.0.8.tar", last modified: Sun May  7 00:03:11 2023, max compression
+gzip compressed data, was "FeatureInsight-0.0.9.tar", last modified: Thu Jun  1 11:54:39 2023, max compression
```

## Comparing `FeatureInsight-0.0.8.tar` & `FeatureInsight-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.505610 FeatureInsight-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.486610 FeatureInsight-0.0.8/FeatureInsight/
--rw-rw-rw-   0        0        0     4287 2023-05-06 23:52:10.000000 FeatureInsight-0.0.8/FeatureInsight/EDA_Investigation.py
--rw-rw-rw-   0        0        0      442 2023-05-07 00:01:56.000000 FeatureInsight-0.0.8/FeatureInsight/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.503610 FeatureInsight-0.0.8/FeatureInsight/shell/
--rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.8/FeatureInsight/shell/__init__.py
--rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.8/FeatureInsight/shell/usage.py
--rw-rw-rw-   0        0        0     2590 2023-05-06 22:28:33.000000 FeatureInsight-0.0.8/FeatureInsight/structure_Investigation.py
--rw-rw-rw-   0        0        0     1498 2023-05-06 23:06:50.000000 FeatureInsight-0.0.8/FeatureInsight/untitled.py
-drwxrwxrwx   0        0        0        0 2023-05-07 00:03:11.500610 FeatureInsight-0.0.8/FeatureInsight.egg-info/
--rw-rw-rw-   0        0        0      854 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      162 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-07 00:03:11.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.8/FeatureInsight.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      854 2023-05-07 00:03:11.504610 FeatureInsight-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-05-07 00:03:06.000000 FeatureInsight-0.0.8/README.md
--rw-rw-rw-   0        0        0      161 2023-05-06 22:52:29.000000 FeatureInsight-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 00:03:11.505610 FeatureInsight-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:54:39.370293 FeatureInsight-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-01 11:54:39.358324 FeatureInsight-0.0.9/FeatureInsight/
+-rw-rw-rw-   0        0        0     4625 2023-05-16 11:10:18.000000 FeatureInsight-0.0.9/FeatureInsight/EDA_Investigation.py
+-rw-rw-rw-   0        0        0      442 2023-06-01 11:53:54.000000 FeatureInsight-0.0.9/FeatureInsight/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:54:39.369296 FeatureInsight-0.0.9/FeatureInsight/shell/
+-rw-rw-rw-   0        0        0       66 2023-05-06 21:36:44.000000 FeatureInsight-0.0.9/FeatureInsight/shell/__init__.py
+-rw-rw-rw-   0        0        0      206 2023-05-06 21:36:44.000000 FeatureInsight-0.0.9/FeatureInsight/shell/usage.py
+-rw-rw-rw-   0        0        0     3439 2023-06-01 11:49:42.000000 FeatureInsight-0.0.9/FeatureInsight/structure_Investigation.py
+-rw-rw-rw-   0        0        0     1498 2023-05-06 23:06:50.000000 FeatureInsight-0.0.9/FeatureInsight/untitled.py
+drwxrwxrwx   0        0        0        0 2023-06-01 11:54:39.367305 FeatureInsight-0.0.9/FeatureInsight.egg-info/
+-rw-rw-rw-   0        0        0      975 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      162 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-01 11:54:39.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 21:37:38.000000 FeatureInsight-0.0.9/FeatureInsight.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1083 2023-05-06 21:32:28.000000 FeatureInsight-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      181 2023-05-06 21:36:43.000000 FeatureInsight-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      975 2023-06-01 11:54:39.370293 FeatureInsight-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      521 2023-06-01 11:52:04.000000 FeatureInsight-0.0.9/README.md
+-rw-rw-rw-   0        0        0      161 2023-05-06 22:52:29.000000 FeatureInsight-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 11:54:39.370293 FeatureInsight-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2023-05-06 22:10:43.000000 FeatureInsight-0.0.9/setup.py
```

### Comparing `FeatureInsight-0.0.8/FeatureInsight/EDA_Investigation.py` & `FeatureInsight-0.0.9/FeatureInsight/EDA_Investigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,18 +69,19 @@
     """
     num_list, cata_list, other_list = generate_lists(train_df, collist)
     
     # Plot the distribution for numerical features
     klib.dist_plot(train_df[num_list])
 
     # Plot the distribution for categorical features
-    if mode == 'bar':
-        plot_categorical_distribution(train_df, cata_list)
-    elif mode == 'pie':
-        plot_categorical_pie_charts(train_df, cata_list)
+    if cata_list!=[]:
+        if mode == 'bar':
+            plot_categorical_distribution(train_df, cata_list)
+        elif mode == 'pie':
+            plot_categorical_pie_charts(train_df, cata_list)
 
     # Print the other features
     print("Other features: ", other_list)
 
 def generate_lists(df, collist):
     num_list = []
     cata_list = []
@@ -98,14 +99,20 @@
 
 
 def plot_categorical_distribution(df, cata_list):
     ncols = 3
     nrows = (len(cata_list) + ncols - 1) // ncols
     fig, axs = plt.subplots(nrows, ncols, figsize=(15, nrows * 5), constrained_layout=True)
 
+    # Adjust for 1D and 2D axs array.
+    if nrows == 1:
+        axs = axs[np.newaxis, :]
+    elif ncols == 1:
+        axs = axs[:, np.newaxis]
+        
     for idx, col in enumerate(cata_list):
         row, col_idx = divmod(idx, ncols)
         sns.countplot(x=col, data=df, ax=axs[row, col_idx])
         axs[row, col_idx].set_title(f"{col} Distribution")
 
     # Remove unused subplots
     for idx in range(len(cata_list), nrows * ncols):
@@ -115,19 +122,25 @@
     plt.show()
     
 def plot_categorical_pie_charts(df, cata_list):
     ncols = 3
     nrows = (len(cata_list) + ncols - 1) // ncols
     fig, axs = plt.subplots(nrows, ncols, figsize=(15, nrows * 5), constrained_layout=True)
 
+    # Adjust for 1D and 2D axs array.
+    if nrows == 1:
+        axs = axs[np.newaxis, :]
+    elif ncols == 1:
+        axs = axs[:, np.newaxis]
+
     for idx, col in enumerate(cata_list):
         row, col_idx = divmod(idx, ncols)
-        df[col].value_counts().plot.pie(autopct='%1.1f%%', ax=axs[row, col_idx])
+        df[col].value_counts().plot.pie(autopct='%1.1f%%', ax=axs[row, col_idx]) #e
         axs[row, col_idx].set_ylabel('')
         axs[row, col_idx].set_title(f"{col} Distribution")
 
     # Remove unused subplots
     for idx in range(len(cata_list), nrows * ncols):
         row, col_idx = divmod(idx, ncols)
         fig.delaxes(axs[row, col_idx])
 
-    plt.show()
+    plt.show()
```

### Comparing `FeatureInsight-0.0.8/FeatureInsight/structure_Investigation.py` & `FeatureInsight-0.0.9/FeatureInsight/structure_Investigation.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,42 @@
 import os
 from PIL import Image
 import cv2
 from tqdm import tqdm
 from tabulate import tabulate
 from feature_engine.encoding import *
 
+ 
+from tabulate import tabulate
+import pandas as pd
+ 
+ 
+import re
+
+class PrintableDataFrame(pd.DataFrame):
+
+    def print(self):
+        print(tabulate(self, headers='keys', tablefmt='psql'))
+
+    def sort(self, col):
+        sorted_df = self.copy()  # Make a copy of the DataFrame
+
+        # Extract the number from the unique count string and create a separate column for sorting
+        sorted_df['sort_column'] = sorted_df[col].apply(lambda x: int(re.findall(r'\d+', x)[0]) if re.findall(r'\d+', x) else None)
+
+        # Sort the DataFrame based on the extracted number in descending order
+        sorted_df = sorted_df.sort_values(by='sort_column', ascending=False)
+
+        # Remove the temporary sort column
+        sorted_df = sorted_df.drop(columns='sort_column')
+
+        sorted_printable_df = PrintableDataFrame(sorted_df)
+        sorted_printable_df.print()
+
+
 def struct_Investigation(df): 
    """plot Overview Information about datatype, variable type, shape, examples
    Detailed explanation 
    Args:  
        df: train in dataframe
        img: ['img1','img1'] the image feature name
    Returns:
@@ -27,15 +55,15 @@
      df.img_list=[]
    print("There are {} instances, {} cols in total".format(df.iloc[:,0].count(),df.iloc[0,:].count()))
    info = pd.DataFrame( columns=["variable","dtype","measure_scales","Unique Count","Null Count","thumbnail"])
    info.variable=df.columns
    info=info.set_index('variable')
 
    # info.i=df.dtype
-   for fea in list(df.columns):
+   for fea in tqdm(list(df.columns)):
        info.loc[fea,"Null Count"]=str(df[fea].isnull().sum())+"("+str(df[fea].isnull().sum()/df[fea].shape[0]*100)+"%)"
        info.loc[fea,"dtype"]=str(df[fea].dtypes)         
        if str(df[fea].dtypes)=='object':
            info.loc[fea,"dtype"]=str(set([type(x).__name__ for x in df[fea]]))    
        #info.i=df.shape
        #info.loc[fea,"shape"]=list(set([x.shape for x in df[fea]]))    
 
@@ -62,10 +90,10 @@
                info.loc[fea,"measure_scales"]="numerical Data"
 
        else:  
            info.loc[fea,"measure_scales"]="others"
 
        #info.i=df.cardinality
        info.loc[fea,"Unique Count"]= str(df[fea].nunique())+ "({p:.2f}%) of total".format(p=df[fea].nunique()/df[fea].count()*100)
-   print(tabulate(info, headers='keys', tablefmt='psql'))
-   return info
+        
+   return PrintableDataFrame(info)
```

### Comparing `FeatureInsight-0.0.8/FeatureInsight/untitled.py` & `FeatureInsight-0.0.9/FeatureInsight/untitled.py`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.8/FeatureInsight.egg-info/PKG-INFO` & `FeatureInsight-0.0.9/FeatureInsight.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.8
+Version: 0.0.9
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,12 +19,19 @@
 
 # 如何使用？
 
 
 from FeatureInsight import struct_Investigation,univar_dis,bivar_dis
 
 
+EDA: Structure
+summary=struct_Investigation(df)  
+summary.print()
+summary.sort('Unique Count')	
+
+
+EDA: statistics
+
 univar_dis(df,df.columns,mode="pie")
 univar_dis(df,df.columns)
-
 bivar_dis(df,[["Age","Drug"],["Sex","BP"],["K","Drug"]],mode="Bar")
 bivar_dis(df,[["Age","Drug"],["Sex","BP"],["K","Drug"]],mode="Line")
```

### Comparing `FeatureInsight-0.0.8/FeatureInsight.egg-info/SOURCES.txt` & `FeatureInsight-0.0.9/FeatureInsight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.8/LICENSE` & `FeatureInsight-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FeatureInsight-0.0.8/PKG-INFO` & `FeatureInsight-0.0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FeatureInsight
-Version: 0.0.8
+Version: 0.0.9
 Summary: project description
 Home-page: https://github.com/px39n/FeatureInsight
 Author: px39n
 Author-email: isxzl39@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,12 +19,19 @@
 
 # 如何使用？
 
 
 from FeatureInsight import struct_Investigation,univar_dis,bivar_dis
 
 
+EDA: Structure
+summary=struct_Investigation(df)  
+summary.print()
+summary.sort('Unique Count')	
+
+
+EDA: statistics
+
 univar_dis(df,df.columns,mode="pie")
 univar_dis(df,df.columns)
-
 bivar_dis(df,[["Age","Drug"],["Sex","BP"],["K","Drug"]],mode="Bar")
 bivar_dis(df,[["Age","Drug"],["Sex","BP"],["K","Drug"]],mode="Line")
```

### Comparing `FeatureInsight-0.0.8/setup.py` & `FeatureInsight-0.0.9/setup.py`

 * *Files identical despite different names*

