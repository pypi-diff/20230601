# Comparing `tmp/bmtool-0.3.5.tar.gz` & `tmp/bmtool-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.5.tar", last modified: Tue May 23 16:27:31 2023, max compression
+gzip compressed data, was "bmtool-0.3.6.tar", last modified: Wed May 31 22:11:47 2023, max compression
```

## Comparing `bmtool-0.3.5.tar` & `bmtool-0.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.053040 bmtool-0.3.5/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.5/LICENSE
--rw-rw-rw-   0        0        0    16777 2023-05-23 16:27:31.050037 bmtool-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.005174 bmtool-0.3.5/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.5/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.5/bmtool/__main__.py
--rw-rw-rw-   0        0        0    25442 2023-03-17 15:40:34.000000 bmtool-0.3.5/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.033685 bmtool-0.3.5/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.5/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.5/bmtool/manage.py
--rw-rw-rw-   0        0        0    10440 2023-03-17 15:16:10.000000 bmtool-0.3.5/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.5/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.042872 bmtool-0.3.5/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.5/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.047857 bmtool-0.3.5/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.5/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    51814 2023-05-23 16:25:45.000000 bmtool-0.3.5/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.027584 bmtool-0.3.5/bmtool.egg-info/
--rw-rw-rw-   0        0        0    16777 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 16:27:31.053040 bmtool-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-05-23 16:26:06.000000 bmtool-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.445024 bmtool-0.3.6/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0    16777 2023-05-31 22:11:47.443958 bmtool-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.378720 bmtool-0.3.6/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.6/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.6/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    28949 2023-05-31 22:09:17.000000 bmtool-0.3.6/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.425298 bmtool-0.3.6/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.6/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.6/bmtool/manage.py
+-rw-rw-rw-   0        0        0    12289 2023-05-31 21:35:05.000000 bmtool-0.3.6/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.6/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.433557 bmtool-0.3.6/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.6/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.441609 bmtool-0.3.6/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.6/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.6/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-29 23:57:07.000000 bmtool-0.3.6/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-05-31 22:11:47.412643 bmtool-0.3.6/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    16777 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-31 22:11:46.000000 bmtool-0.3.6/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 22:11:45.000000 bmtool-0.3.6/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 22:11:47.445024 bmtool-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-05-31 22:10:51.000000 bmtool-0.3.6/setup.py
```

### Comparing `bmtool-0.3.5/LICENSE` & `bmtool-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/PKG-INFO` & `bmtool-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.5
+Version: 0.3.6
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.5/README.md` & `bmtool-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/__main__.py` & `bmtool-0.3.6/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/bmplot.py` & `bmtool-0.3.6/bmtool/bmplot.py`

 * *Files 10% similar despite different names*

```diff
@@ -401,14 +401,105 @@
 
     if save_file:
         plt.savefig(save_file)
 
     return
 
 
+def cell_rotation_3d(**kwargs):
+    populations_list = kwargs["populations"]
+    config = kwargs["config"]
+    group_keys = kwargs["group_by"]
+    title = kwargs["title"]
+    save_file = kwargs["save_file"]
+    quiver_length = kwargs["quiver_length"]
+    arrow_length_ratio = kwargs["arrow_length_ratio"]
+    group = kwargs["group"]
+    max_cells = kwargs["max_cells"]
+
+    nodes = util.load_nodes_from_config(config)
+
+    if 'all' in populations_list:
+        populations = list(nodes)
+    else:
+        populations = populations_list.split(",")
+
+    group_keys = group_keys.split(",")
+    group_keys += (len(populations)-len(group_keys)) * ["node_type_id"] #Extend the array to default values if not enough given
+    fig = plt.figure(figsize=(10,10))
+    ax = Axes3D(fig)
+    handles = []
+    for nodes_key,group_key in zip(list(nodes),group_keys):
+        if 'all' not in populations and nodes_key not in populations:
+            continue
+            
+        nodes_df = nodes[nodes_key]
+
+        if group_key is not None:
+            if group_key not in nodes_df:
+                raise Exception('Could not find column {}'.format(group_key))
+            groupings = nodes_df.groupby(group_key)
+
+            n_colors = nodes_df[group_key].nunique()
+            color_norm = colors.Normalize(vmin=0, vmax=(n_colors-1))
+            scalar_map = cmx.ScalarMappable(norm=color_norm, cmap='hsv')
+            color_map = [scalar_map.to_rgba(i) for i in range(0, n_colors)]
+        else:
+            groupings = [(None, nodes_df)]
+            color_map = ['blue']
+
+        cells_plotted = 0
+        for color, (group_name, group_df) in zip(color_map, groupings):
+            # if we selected a group and it's not in the list continue
+            if group and group_name not in group.split(","):
+                continue
+
+            if "pos_x" not in group_df: #could also check model type == virtual
+                continue #can't plot them if there isn't an xy coordinate (may be virtual)
+
+            # if we exceed the max cells, stop plotting or limit
+            if cells_plotted >= max_cells:
+                continue
+            if len(group_df) + cells_plotted > max_cells:
+                total_remaining = max_cells - cells_plotted
+                group_df = group_df[:total_remaining]
+            cells_plotted += len(group_df)
+
+            X = group_df["pos_x"]
+            Y = group_df["pos_y"]
+            Z = group_df["pos_z"]
+            U = group_df.get("rotation_angle_xaxis") 
+            V = group_df.get("rotation_angle_yaxis")
+            W = group_df.get("rotation_angle_zaxis")
+            if U is None:
+                U = np.zeros(len(X))
+            if V is None:
+                V = np.zeros(len(Y))
+            if W is None:
+                W = np.zeros(len(Z))
+            
+            #Convert to arrow direction
+            from scipy.spatial.transform import Rotation as R
+            uvw = pd.DataFrame([U,V,W]).T
+            rots = R.from_euler('zyx', uvw).as_rotvec().T
+            h = ax.quiver(X, Y, Z, rots[0],rots[1],rots[2],color=color,label=group_name, arrow_length_ratio = arrow_length_ratio, length=quiver_length)
+            ax.scatter(X,Y,Z,color=color,label=group_name)
+            handles.append(h)
+    if not handles:
+        return
+    plt.title(title)
+    plt.legend(handles=handles)
+    
+    plt.draw()
+
+    if save_file:
+        plt.savefig(save_file)
+
+    return
+
 def plot_network_graph(config=None,nodes=None,edges=None,title=None,sources=None, targets=None, sids=None, tids=None, no_prepend_pop=False,save_file=None,edge_property='model_template'):
     
     if not sources or not targets:
         raise Exception("Sources or targets not defined")
     sources = sources.split(",")
     targets = targets.split(",")
     if sids:
```

### Comparing `bmtool-0.3.5/bmtool/debug/commands.py` & `bmtool-0.3.6/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/manage.py` & `bmtool-0.3.6/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/plot_commands.py` & `bmtool-0.3.6/bmtool/plot_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from clint.textui import puts, colored, indent
 from .bmplot import (connection_matrix, percent_connection_matrix,
                 divergence_connection_matrix,plot_3d_positions,
                 edge_histogram_matrix,plot_network_graph,
                 raster,plot_report_default,probability_connection_matrix,
                 sim_setup,plot_I_clamps,plot_basic_cell_info,
-                plot_inspikes)
+                plot_inspikes, cell_rotation_3d)
 import matplotlib.pyplot as plt
 
 @click.group('plot')
 @click.option('--config', type=click.Path(), default='./simulation_config.json', help='Configuration file to use, default: "simulation_config.json"')
 @click.option('--no-display', is_flag=True, default=False, help='When set there will be no plot displayed, useful for saving plots')
 @click.pass_context
 def cli(ctx, config, no_display):
@@ -114,14 +114,45 @@
 @click.option('--edge-property', type=click.STRING, default='model_template', help="Edge property to define connections [default:model_template]")
 @click.pass_context
 def connection_network_graph(ctx,edge_property):
     plot_network_graph(ctx.obj['config'],**ctx.obj['connection'],edge_property=edge_property)
     if ctx.obj['display']:
         plt.show()
 
+@click.group('cell', help='Plot information regarding cells in the model')
+@click.option('--title', type=click.STRING, default=None, help="change the plot's title")
+@click.option('--save-file', type=click.STRING, default=None, help="save plot to path supplied")
+@click.pass_context
+def cell(ctx,title,save_file):
+
+    ctx.obj["cell"] = {
+        'title':title,
+        'save_file':save_file
+    }
+    
+@cell.command('rotation',help="Plot a 3d plot for cell rotation")
+@click.option('--populations', type=click.STRING, default='all', help="comma separated list of populations to plot [default:all]")
+@click.option('--group-by', type=click.STRING, default='node_type_id', help="comma separated list of identifiers [default: node_type_id] (pop_name is a good one)")
+@click.option('--group', type=click.STRING, default=None, help="Conditional for cell selection (comma delimited). Eg if group-by was pop_name group would be PNc [default:None]")
+@click.option('--max-cells', type=click.INT, default=None, help="max number of cells to display")
+@click.option('--quiver-length', type=click.FLOAT, default=10, help="how long the arrows should be [default: 10]")
+@click.option('--arrow-length-ratio', type=click.FLOAT, default=0.2, help="ratio for the arrow of the quiver [default: 0.2]")
+@click.pass_context
+def rotation_3d(ctx,populations,group_by,group,max_cells,quiver_length,arrow_length_ratio):
+    cell_rotation_3d(config=ctx.obj['config'],**ctx.obj['cell'],
+                     populations=populations,
+                     group_by=group_by,
+                     group=group,
+                     max_cells=max_cells,
+                     quiver_length=quiver_length,
+                     arrow_length_ratio=arrow_length_ratio)
+    if ctx.obj['display']:
+        plt.show()
+
+
 @cli.command('positions', help="Plot cell positions for a given set of populations")
 @click.option('--title', type=click.STRING, default='Cell 3D Positions', help="change the plot's title")
 @click.option('--populations', type=click.STRING, default='all', help="comma separated list of populations to plot [default:all]")
 @click.option('--group-by', type=click.STRING, default='node_type_id', help="comma separated list of identifiers [default: node_type_id] (pop_name is a good one)")
 @click.option('--save-file', type=click.STRING, default=None, help="save plot to path supplied [default:None]")
 @click.pass_context
 def plot_positions(ctx, title, populations, group_by, save_file):
@@ -187,10 +218,11 @@
 def Spikes(ctx):
     plot_inspikes(fp=ctx.obj['config'])
     if ctx.obj['display']:
         plt.show()
 
 
 cli.add_command(connection)
+cli.add_command(cell)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `bmtool-0.3.5/bmtool/singlecell.py` & `bmtool-0.3.6/bmtool/singlecell.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/util/commands.py` & `bmtool-0.3.6/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/util/neuron/celltuner.py` & `bmtool-0.3.6/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool/util/util.py` & `bmtool-0.3.6/bmtool/util/util.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/bmtool.egg-info/PKG-INFO` & `bmtool-0.3.6/bmtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.5
+Version: 0.3.6
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.5/bmtool.egg-info/SOURCES.txt` & `bmtool-0.3.6/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.5/setup.py` & `bmtool-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.5",
+    version="0.3.6",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

