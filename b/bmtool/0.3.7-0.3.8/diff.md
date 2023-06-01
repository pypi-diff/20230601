# Comparing `tmp/bmtool-0.3.7.tar.gz` & `tmp/bmtool-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.7.tar", last modified: Wed May 31 22:26:29 2023, max compression
+gzip compressed data, was "bmtool-0.3.8.tar", last modified: Thu Jun  1 14:39:14 2023, max compression
```

## Comparing `bmtool-0.3.7.tar` & `bmtool-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.910262 bmtool-0.3.7/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.7/LICENSE
--rw-rw-rw-   0        0        0    16777 2023-05-31 22:26:29.908266 bmtool-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.849167 bmtool-0.3.7/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.7/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.7/bmtool/__main__.py
--rw-rw-rw-   0        0        0    28949 2023-05-31 22:22:04.000000 bmtool-0.3.7/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.892298 bmtool-0.3.7/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.7/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.7/bmtool/manage.py
--rw-rw-rw-   0        0        0    12315 2023-05-31 22:22:30.000000 bmtool-0.3.7/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.7/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.901193 bmtool-0.3.7/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.7/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.905037 bmtool-0.3.7/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.7/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.7/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.7/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-31 22:26:29.881944 bmtool-0.3.7/bmtool.egg-info/
--rw-rw-rw-   0        0        0    16777 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 22:26:28.000000 bmtool-0.3.7/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 22:26:29.910262 bmtool-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-05-31 22:23:43.000000 bmtool-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.737986 bmtool-0.3.8/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0    17751 2023-06-01 14:39:14.735984 bmtool-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    17006 2023-05-31 22:34:19.000000 bmtool-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.655336 bmtool-0.3.8/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.8/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.8/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    29471 2023-06-01 14:33:49.000000 bmtool-0.3.8/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.697624 bmtool-0.3.8/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.8/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.8/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12528 2023-06-01 14:19:08.000000 bmtool-0.3.8/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.8/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.716735 bmtool-0.3.8/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.8/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.732984 bmtool-0.3.8/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.8/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.8/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.8/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:39:14.678339 bmtool-0.3.8/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    17751 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-06-01 14:39:13.000000 bmtool-0.3.8/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 14:39:12.000000 bmtool-0.3.8/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:39:14.738129 bmtool-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-06-01 14:38:41.000000 bmtool-0.3.8/setup.py
```

### Comparing `bmtool-0.3.7/LICENSE` & `bmtool-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/PKG-INFO` & `bmtool-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.7
+Version: 0.3.8
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -338,14 +338,42 @@
 bmtool plot connection --sources hippocampus --targets hippocampus --no-prepend-pop --sids pop_name --tids pop_name prob --bins 10 --line --verbose
 ```
 
 This will plot cells in the `hippocampus` network, using the `pop_name` as the cell identifier. There will be `10` bins created to group the cell distances. A `line` plot will be generated instead of the default `bar` chart. All values for each plot will be printed to the console due to the `verbose` flag.
 
 All  `point_process` cell types will be ignored since they do not have physical locations.
 
+### Plot 3d cell location and rotation
+Plot the location and rotation of your cells. Plot all of your cells with a single command
+```
+bmtool plot cell rotation
+```
+![bmtool](./figures/rotation3d_1.png "3d Rotation Figure")
+
+Customize your plot by limiting the cells you want or selecting a max number of cells to plot.
+```
+bmtool plot --config simulation_configECP.json cell rotation --group-by pop_name --group CR --max-cells 100 --quiver-length 100 --arrow-length-ratio 0.25
+```
+![bmtool](./figures/rotation3d_2.png "3d Rotation Figure")
+
+Code
+```
+from bmtool import
+from bmtool import bmplot
+
+bmplot.cell_rotation_3d(config=config,
+                     populations=populations,
+                     group_by=group_by,
+                     group=group,
+                     title=title,
+                     max_cells=max_cells,
+                     quiver_length=quiver_length,
+                     arrow_length_ratio=arrow_length_ratio)
+```
+
 ### Plotting Current Clamp and Spike Train Info
 To plot all current clamp info involved in a simulation, use the following command (uses 'simulation_config.json' as default)
 ```
 bmtool plot --config simulation_config_foo.json iclamp
 ```
 
 To plot all spike trains and their target cells,
```

### Comparing `bmtool-0.3.7/README.md` & `bmtool-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,42 @@
 bmtool plot connection --sources hippocampus --targets hippocampus --no-prepend-pop --sids pop_name --tids pop_name prob --bins 10 --line --verbose
 ```
 
 This will plot cells in the `hippocampus` network, using the `pop_name` as the cell identifier. There will be `10` bins created to group the cell distances. A `line` plot will be generated instead of the default `bar` chart. All values for each plot will be printed to the console due to the `verbose` flag.
 
 All  `point_process` cell types will be ignored since they do not have physical locations.
 
+### Plot 3d cell location and rotation
+Plot the location and rotation of your cells. Plot all of your cells with a single command
+```
+bmtool plot cell rotation
+```
+![bmtool](./figures/rotation3d_1.png "3d Rotation Figure")
+
+Customize your plot by limiting the cells you want or selecting a max number of cells to plot.
+```
+bmtool plot --config simulation_configECP.json cell rotation --group-by pop_name --group CR --max-cells 100 --quiver-length 100 --arrow-length-ratio 0.25
+```
+![bmtool](./figures/rotation3d_2.png "3d Rotation Figure")
+
+Code
+```
+from bmtool import
+from bmtool import bmplot
+
+bmplot.cell_rotation_3d(config=config,
+                     populations=populations,
+                     group_by=group_by,
+                     group=group,
+                     title=title,
+                     max_cells=max_cells,
+                     quiver_length=quiver_length,
+                     arrow_length_ratio=arrow_length_ratio)
+```
+
 ### Plotting Current Clamp and Spike Train Info
 To plot all current clamp info involved in a simulation, use the following command (uses 'simulation_config.json' as default)
 ```
 bmtool plot --config simulation_config_foo.json iclamp
 ```
 
 To plot all spike trains and their target cells,
```

### Comparing `bmtool-0.3.7/bmtool/__main__.py` & `bmtool-0.3.8/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/bmplot.py` & `bmtool-0.3.8/bmtool/bmplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,20 +405,21 @@
     return
 
 
 def cell_rotation_3d(**kwargs):
     populations_list = kwargs["populations"]
     config = kwargs["config"]
     group_keys = kwargs["group_by"]
-    title = kwargs["title"]
+    title = kwargs.get("title")
     save_file = kwargs["save_file"]
     quiver_length = kwargs["quiver_length"]
     arrow_length_ratio = kwargs["arrow_length_ratio"]
     group = kwargs["group"]
-    max_cells = kwargs["max_cells"]
+    max_cells = kwargs.get("max_cells",999999999)
+    init_vector = kwargs.get("init_vector","1,0,0")
 
     nodes = util.load_nodes_from_config(config)
 
     if 'all' in populations_list:
         populations = list(nodes)
     else:
         populations = populations_list.split(",")
@@ -476,15 +477,22 @@
                 V = np.zeros(len(Y))
             if W is None:
                 W = np.zeros(len(Z))
             
             #Convert to arrow direction
             from scipy.spatial.transform import Rotation as R
             uvw = pd.DataFrame([U,V,W]).T
-            rots = R.from_euler('zyx', uvw).as_rotvec().T
+            init_vector = init_vector.split(',')
+            init_vector = np.repeat([init_vector],len(X),axis=0)
+            # To get the final cell orientation after rotation, 
+            # you need to use function Rotaion.apply(init_vec), 
+            # where init_vec is a vector of the initial orientation of a cell
+            rots = R.from_euler('xyz', uvw).apply(init_vector.astype(float))
+            rots = R.from_euler('xyz', pd.DataFrame([rots[:,0],rots[:,1],rots[:,2]]).T).as_rotvec().T
+
             h = ax.quiver(X, Y, Z, rots[0],rots[1],rots[2],color=color,label=group_name, arrow_length_ratio = arrow_length_ratio, length=quiver_length)
             ax.scatter(X,Y,Z,color=color,label=group_name)
             handles.append(h)
     if not handles:
         return
     plt.title(title)
     plt.legend(handles=handles)
```

### Comparing `bmtool-0.3.7/bmtool/debug/commands.py` & `bmtool-0.3.8/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/manage.py` & `bmtool-0.3.8/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/plot_commands.py` & `bmtool-0.3.8/bmtool/plot_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,23 +132,25 @@
 @cell.command('rotation',help="Plot a 3d plot for cell rotation")
 @click.option('--populations', type=click.STRING, default='all', help="comma separated list of populations to plot [default:all]")
 @click.option('--group-by', type=click.STRING, default='node_type_id', help="comma separated list of identifiers [default: node_type_id] (pop_name is a good one)")
 @click.option('--group', type=click.STRING, default=None, help="Conditional for cell selection (comma delimited). Eg if group-by was pop_name group would be PNc [default:None]")
 @click.option('--max-cells', type=click.INT, default=999999999, help="max number of cells to display [default: 999999999]")
 @click.option('--quiver-length', type=click.FLOAT, default=10, help="how long the arrows should be [default: 10]")
 @click.option('--arrow-length-ratio', type=click.FLOAT, default=0.2, help="ratio for the arrow of the quiver [default: 0.2]")
+@click.option('--init-vector', type=click.STRING, default="1,0,0", help="comma delimited initial rotation vector specified by pt3dadd [default: 0,0,1]")
 @click.pass_context
-def rotation_3d(ctx,populations,group_by,group,max_cells,quiver_length,arrow_length_ratio):
+def rotation_3d(ctx,populations,group_by,group,max_cells,quiver_length,arrow_length_ratio,init_vector):
     cell_rotation_3d(config=ctx.obj['config'],**ctx.obj['cell'],
                      populations=populations,
                      group_by=group_by,
                      group=group,
                      max_cells=max_cells,
                      quiver_length=quiver_length,
-                     arrow_length_ratio=arrow_length_ratio)
+                     arrow_length_ratio=arrow_length_ratio,
+                     init_vector=init_vector)
     if ctx.obj['display']:
         plt.show()
 
 
 @cli.command('positions', help="Plot cell positions for a given set of populations")
 @click.option('--title', type=click.STRING, default='Cell 3D Positions', help="change the plot's title")
 @click.option('--populations', type=click.STRING, default='all', help="comma separated list of populations to plot [default:all]")
```

### Comparing `bmtool-0.3.7/bmtool/singlecell.py` & `bmtool-0.3.8/bmtool/singlecell.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/util/commands.py` & `bmtool-0.3.8/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/util/neuron/celltuner.py` & `bmtool-0.3.8/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool/util/util.py` & `bmtool-0.3.8/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/bmtool.egg-info/PKG-INFO` & `bmtool-0.3.8/bmtool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.7
+Version: 0.3.8
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -338,14 +338,42 @@
 bmtool plot connection --sources hippocampus --targets hippocampus --no-prepend-pop --sids pop_name --tids pop_name prob --bins 10 --line --verbose
 ```
 
 This will plot cells in the `hippocampus` network, using the `pop_name` as the cell identifier. There will be `10` bins created to group the cell distances. A `line` plot will be generated instead of the default `bar` chart. All values for each plot will be printed to the console due to the `verbose` flag.
 
 All  `point_process` cell types will be ignored since they do not have physical locations.
 
+### Plot 3d cell location and rotation
+Plot the location and rotation of your cells. Plot all of your cells with a single command
+```
+bmtool plot cell rotation
+```
+![bmtool](./figures/rotation3d_1.png "3d Rotation Figure")
+
+Customize your plot by limiting the cells you want or selecting a max number of cells to plot.
+```
+bmtool plot --config simulation_configECP.json cell rotation --group-by pop_name --group CR --max-cells 100 --quiver-length 100 --arrow-length-ratio 0.25
+```
+![bmtool](./figures/rotation3d_2.png "3d Rotation Figure")
+
+Code
+```
+from bmtool import
+from bmtool import bmplot
+
+bmplot.cell_rotation_3d(config=config,
+                     populations=populations,
+                     group_by=group_by,
+                     group=group,
+                     title=title,
+                     max_cells=max_cells,
+                     quiver_length=quiver_length,
+                     arrow_length_ratio=arrow_length_ratio)
+```
+
 ### Plotting Current Clamp and Spike Train Info
 To plot all current clamp info involved in a simulation, use the following command (uses 'simulation_config.json' as default)
 ```
 bmtool plot --config simulation_config_foo.json iclamp
 ```
 
 To plot all spike trains and their target cells,
```

### Comparing `bmtool-0.3.7/bmtool.egg-info/SOURCES.txt` & `bmtool-0.3.8/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.7/setup.py` & `bmtool-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.7",
+    version="0.3.8",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

