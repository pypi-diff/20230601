# Comparing `tmp/bmtool-0.3.8.tar.gz` & `tmp/bmtool-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.8.tar", last modified: Thu Jun  1 14:39:14 2023, max compression
+gzip compressed data, was "bmtool-0.3.9.tar", last modified: Thu Jun  1 20:42:37 2023, max compression
```

## Comparing `bmtool-0.3.8.tar` & `bmtool-0.3.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.737986 bmtool-0.3.8/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.8/LICENSE
--rw-rw-rw-   0        0        0    17751 2023-06-01 14:39:14.735984 bmtool-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.655336 bmtool-0.3.8/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.8/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.8/bmtool/__main__.py
--rw-rw-rw-   0        0        0    29471 2023-06-01 14:33:49.000000 bmtool-0.3.8/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.697624 bmtool-0.3.8/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.8/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.8/bmtool/manage.py
--rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.3.8/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.8/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.716735 bmtool-0.3.8/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.8/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.732984 bmtool-0.3.8/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.8/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.8/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.678339 bmtool-0.3.8/bmtool.egg-info/
--rw-rw-rw-   0        0        0    17751 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-06-01 14:39:13.000000 bmtool-0.3.8/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:39:14.738129 bmtool-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-06-01 14:38:41.000000 bmtool-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.656518 bmtool-0.3.9/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0    17751 2023-06-01 20:42:37.654472 bmtool-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.600814 bmtool-0.3.9/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.9/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.9/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    29723 2023-06-01 20:21:45.000000 bmtool-0.3.9/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.641929 bmtool-0.3.9/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.9/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.9/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.3.9/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.9/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.647922 bmtool-0.3.9/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.9/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.652467 bmtool-0.3.9/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.9/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.9/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.9/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 20:42:37.620939 bmtool-0.3.9/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    17751 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-06-01 20:42:36.000000 bmtool-0.3.9/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 20:42:35.000000 bmtool-0.3.9/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 20:42:37.657679 bmtool-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-06-01 20:40:18.000000 bmtool-0.3.9/setup.py
```

### Comparing `bmtool-0.3.8/LICENSE` & `bmtool-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/PKG-INFO` & `bmtool-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.8
+Version: 0.3.9
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.8/README.md` & `bmtool-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/__main__.py` & `bmtool-0.3.9/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/bmplot.py` & `bmtool-0.3.9/bmtool/bmplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,21 +479,25 @@
                 W = np.zeros(len(Z))
             
             #Convert to arrow direction
             from scipy.spatial.transform import Rotation as R
             uvw = pd.DataFrame([U,V,W]).T
             init_vector = init_vector.split(',')
             init_vector = np.repeat([init_vector],len(X),axis=0)
+            
             # To get the final cell orientation after rotation, 
             # you need to use function Rotaion.apply(init_vec), 
             # where init_vec is a vector of the initial orientation of a cell
-            rots = R.from_euler('xyz', uvw).apply(init_vector.astype(float))
-            rots = R.from_euler('xyz', pd.DataFrame([rots[:,0],rots[:,1],rots[:,2]]).T).as_rotvec().T
+            #rots = R.from_euler('xyz', uvw).apply(init_vector.astype(float))
+            #rots = R.from_euler('xyz', pd.DataFrame([rots[:,0],rots[:,1],rots[:,2]]).T).as_rotvec().T
 
+            rots = R.from_euler('zyx', uvw).apply(init_vector.astype(float)).T
             h = ax.quiver(X, Y, Z, rots[0],rots[1],rots[2],color=color,label=group_name, arrow_length_ratio = arrow_length_ratio, length=quiver_length)
+
+            #h = ax.quiver(X, Y, Z, rots[0],rots[1],rots[2],color=color,label=group_name, arrow_length_ratio = arrow_length_ratio, length=quiver_length)
             ax.scatter(X,Y,Z,color=color,label=group_name)
             handles.append(h)
     if not handles:
         return
     plt.title(title)
     plt.legend(handles=handles)
```

### Comparing `bmtool-0.3.8/bmtool/debug/commands.py` & `bmtool-0.3.9/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/manage.py` & `bmtool-0.3.9/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/plot_commands.py` & `bmtool-0.3.9/bmtool/plot_commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/singlecell.py` & `bmtool-0.3.9/bmtool/singlecell.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/util/commands.py` & `bmtool-0.3.9/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/util/neuron/celltuner.py` & `bmtool-0.3.9/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool/util/util.py` & `bmtool-0.3.9/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/bmtool.egg-info/PKG-INFO` & `bmtool-0.3.9/bmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.8
+Version: 0.3.9
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.8/bmtool.egg-info/SOURCES.txt` & `bmtool-0.3.9/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.8/setup.py` & `bmtool-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.8",
+    version="0.3.9",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

