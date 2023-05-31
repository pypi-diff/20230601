# Comparing `tmp/bmtool-0.3.6.tar.gz` & `tmp/bmtool-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.6.tar", last modified: Wed May 31 22:11:47 2023, max compression
+gzip compressed data, was "bmtool-0.3.7.tar", last modified: Wed May 31 22:26:29 2023, max compression
```

## Comparing `bmtool-0.3.6.tar` & `bmtool-0.3.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.445024 bmtool-0.3.6/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.6/LICENSE
--rw-rw-rw-   0        0        0    16777 2023-05-31 22:11:47.443958 bmtool-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.378720 bmtool-0.3.6/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.6/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.6/bmtool/__main__.py
--rw-rw-rw-   0        0        0    28949 2023-05-31 22:09:17.000000 bmtool-0.3.6/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.425298 bmtool-0.3.6/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.6/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.6/bmtool/manage.py
--rw-rw-rw-   0        0        0    12289 2023-05-31 21:35:05.000000 bmtool-0.3.6/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.6/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.433557 bmtool-0.3.6/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.6/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.441609 bmtool-0.3.6/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.6/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.6/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.412643 bmtool-0.3.6/bmtool.egg-info/
--rw-rw-rw-   0        0        0    16777 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-31 22:11:46.000000 bmtool-0.3.6/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 22:11:47.445024 bmtool-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-05-31 22:10:51.000000 bmtool-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.910262 bmtool-0.3.7/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0    16777 2023-05-31 22:26:29.908266 bmtool-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.849167 bmtool-0.3.7/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.7/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.7/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    28949 2023-05-31 22:22:04.000000 bmtool-0.3.7/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.892298 bmtool-0.3.7/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.7/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.7/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12315 2023-05-31 22:22:30.000000 bmtool-0.3.7/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.7/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.901193 bmtool-0.3.7/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.7/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.905037 bmtool-0.3.7/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.7/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.7/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.881944 bmtool-0.3.7/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    16777 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:26:29.910262 bmtool-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-05-31 22:23:43.000000 bmtool-0.3.7/setup.py
```

### Comparing `bmtool-0.3.6/LICENSE` & `bmtool-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/PKG-INFO` & `bmtool-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.6
+Version: 0.3.7
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.6/README.md` & `bmtool-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/__main__.py` & `bmtool-0.3.7/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/bmplot.py` & `bmtool-0.3.7/bmtool/bmplot.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/debug/commands.py` & `bmtool-0.3.7/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/manage.py` & `bmtool-0.3.7/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/plot_commands.py` & `bmtool-0.3.7/bmtool/plot_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         'save_file':save_file
     }
     
 @cell.command('rotation',help="Plot a 3d plot for cell rotation")
 @click.option('--populations', type=click.STRING, default='all', help="comma separated list of populations to plot [default:all]")
 @click.option('--group-by', type=click.STRING, default='node_type_id', help="comma separated list of identifiers [default: node_type_id] (pop_name is a good one)")
 @click.option('--group', type=click.STRING, default=None, help="Conditional for cell selection (comma delimited). Eg if group-by was pop_name group would be PNc [default:None]")
-@click.option('--max-cells', type=click.INT, default=None, help="max number of cells to display")
+@click.option('--max-cells', type=click.INT, default=999999999, help="max number of cells to display [default: 999999999]")
 @click.option('--quiver-length', type=click.FLOAT, default=10, help="how long the arrows should be [default: 10]")
 @click.option('--arrow-length-ratio', type=click.FLOAT, default=0.2, help="ratio for the arrow of the quiver [default: 0.2]")
 @click.pass_context
 def rotation_3d(ctx,populations,group_by,group,max_cells,quiver_length,arrow_length_ratio):
     cell_rotation_3d(config=ctx.obj['config'],**ctx.obj['cell'],
                      populations=populations,
                      group_by=group_by,
```

### Comparing `bmtool-0.3.6/bmtool/singlecell.py` & `bmtool-0.3.7/bmtool/singlecell.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/util/commands.py` & `bmtool-0.3.7/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/util/neuron/celltuner.py` & `bmtool-0.3.7/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool/util/util.py` & `bmtool-0.3.7/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/bmtool.egg-info/PKG-INFO` & `bmtool-0.3.7/bmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.6
+Version: 0.3.7
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.6/bmtool.egg-info/SOURCES.txt` & `bmtool-0.3.7/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.6/setup.py` & `bmtool-0.3.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.6",
+    version="0.3.7",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

