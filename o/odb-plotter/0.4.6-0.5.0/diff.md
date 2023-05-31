# Comparing `tmp/odb-plotter-0.4.6.tar.gz` & `tmp/odb-plotter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odb-plotter-0.4.6.tar", last modified: Mon Apr 24 22:21:45 2023, max compression
+gzip compressed data, was "odb-plotter-0.5.0.tar", last modified: Wed May 31 22:18:54 2023, max compression
```

## Comparing `odb-plotter-0.4.6.tar` & `odb-plotter-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/
--rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-02-07 20:18:25.000000 odb-plotter-0.4.6/LICENSE
--rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      694 2023-02-20 19:23:31.000000 odb-plotter-0.4.6/README.md
--rw-r--r--   0 clark     (1000) clark     (1000)     1271 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/pyproject.toml
--rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/setup.cfg
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.652210 odb-plotter-0.4.6/src/
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.652210 odb-plotter-0.4.6/src/odb_plotter.egg-info/
--rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/PKG-INFO
--rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/SOURCES.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/dependency_links.txt
--rw-r--r--   0 clark     (1000) clark     (1000)      195 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/requires.txt
--rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-04-24 22:21:45.000000 odb-plotter-0.4.6/src/odb_plotter.egg-info/top_level.txt
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/
--rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-04-24 22:21:35.000000 odb-plotter-0.4.6/src/odbp/__init__.py
--rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-02-08 21:45:04.000000 odb-plotter-0.4.6/src/odbp/__main__.py
--rw-r--r--   0 clark     (1000) clark     (1000)    26212 2023-03-27 21:54:24.000000 odb-plotter-0.4.6/src/odbp/cli.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/data/
--rw-r--r--   0 clark     (1000) clark     (1000)     5191 2023-03-01 19:01:13.000000 odb-plotter-0.4.6/src/odbp/data/config.toml
--rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-03-01 19:01:13.000000 odb-plotter-0.4.6/src/odbp/data/views.toml
--rw-r--r--   0 clark     (1000) clark     (1000)     1366 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/npz_to_hdf.py
--rw-r--r--   0 clark     (1000) clark     (1000)    10839 2023-04-24 22:17:15.000000 odb-plotter-0.4.6/src/odbp/odb.py
--rw-r--r--   0 clark     (1000) clark     (1000)     5111 2023-04-24 22:18:56.000000 odb-plotter-0.4.6/src/odbp/odb_visualizer.py
-drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-04-24 22:21:45.655544 odb-plotter-0.4.6/src/odbp/py2_scripts/
--rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-03-27 18:20:55.000000 odb-plotter-0.4.6/src/odbp/py2_scripts/extract.py
--rw-r--r--   0 clark     (1000) clark     (1000)     8976 2023-03-27 21:54:24.000000 odb-plotter-0.4.6/src/odbp/py2_scripts/odb_to_npz.py
--rw-r--r--   0 clark     (1000) clark     (1000)     2023 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/read_hdf5.py
--rw-r--r--   0 clark     (1000) clark     (1000)    29923 2023-04-24 22:17:15.000000 odb-plotter-0.4.6/src/odbp/state.py
--rw-r--r--   0 clark     (1000) clark     (1000)      914 2023-03-20 21:18:42.000000 odb-plotter-0.4.6/src/odbp/util.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/
+-rw-r--r--   0 clark     (1000) clark     (1000)     1074 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/LICENSE
+-rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      694 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/README.md
+-rw-r--r--   0 clark     (1000) clark     (1000)     1271 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/pyproject.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)       38 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/setup.cfg
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.374586 odb-plotter-0.5.0/src/
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/src/odb_plotter.egg-info/
+-rw-r--r--   0 clark     (1000) clark     (1000)     2569 2023-05-31 22:18:54.000000 odb-plotter-0.5.0/src/odb_plotter.egg-info/PKG-INFO
+-rw-r--r--   0 clark     (1000) clark     (1000)      525 2023-05-31 22:18:54.000000 odb-plotter-0.5.0/src/odb_plotter.egg-info/SOURCES.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        1 2023-05-31 22:18:54.000000 odb-plotter-0.5.0/src/odb_plotter.egg-info/dependency_links.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)      195 2023-05-31 22:18:54.000000 odb-plotter-0.5.0/src/odb_plotter.egg-info/requires.txt
+-rw-r--r--   0 clark     (1000) clark     (1000)        5 2023-05-31 22:18:54.000000 odb-plotter-0.5.0/src/odb_plotter.egg-info/top_level.txt
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/src/odbp/
+-rw-r--r--   0 clark     (1000) clark     (1000)       85 2023-05-25 15:04:32.000000 odb-plotter-0.5.0/src/odbp/__init__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)       59 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/src/odbp/__main__.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    24734 2023-05-25 15:04:32.000000 odb-plotter-0.5.0/src/odbp/cli.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/src/odbp/data/
+-rw-r--r--   0 clark     (1000) clark     (1000)     4872 2023-05-25 15:04:32.000000 odb-plotter-0.5.0/src/odbp/data/config.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)      456 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/src/odbp/data/views.toml
+-rw-r--r--   0 clark     (1000) clark     (1000)     3883 2023-05-30 23:45:50.000000 odb-plotter-0.5.0/src/odbp/npz_to_hdf.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    17191 2023-05-31 01:00:42.000000 odb-plotter-0.5.0/src/odbp/odb.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     4778 2023-05-30 23:47:37.000000 odb-plotter-0.5.0/src/odbp/odb_visualizer.py
+drwxr-xr-x   0 clark     (1000) clark     (1000)        0 2023-05-31 22:18:54.377920 odb-plotter-0.5.0/src/odbp/py2_scripts/
+-rw-r--r--   0 clark     (1000) clark     (1000)     6349 2023-05-25 14:12:43.000000 odb-plotter-0.5.0/src/odbp/py2_scripts/extract.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     7194 2023-05-26 14:57:39.000000 odb-plotter-0.5.0/src/odbp/py2_scripts/odb_to_npz.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     2325 2023-05-31 01:08:07.000000 odb-plotter-0.5.0/src/odbp/read_hdf5.py
+-rw-r--r--   0 clark     (1000) clark     (1000)    28772 2023-05-26 13:32:44.000000 odb-plotter-0.5.0/src/odbp/state.py
+-rw-r--r--   0 clark     (1000) clark     (1000)     1576 2023-05-31 00:54:08.000000 odb-plotter-0.5.0/src/odbp/util.py
```

### Comparing `odb-plotter-0.4.6/LICENSE` & `odb-plotter-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.6/PKG-INFO` & `odb-plotter-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.4.6
+Version: 0.5.0
 Summary: Python3 API for Abaqus FEA .odb Files and related Command Line Visualization Tool, with an Additive Manufacturing Focus
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
```

### Comparing `odb-plotter-0.4.6/README.md` & `odb-plotter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.6/pyproject.toml` & `odb-plotter-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.6/src/odb_plotter.egg-info/PKG-INFO` & `odb-plotter-0.5.0/src/odb_plotter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odb-plotter
-Version: 0.4.6
+Version: 0.5.0
 Summary: Python3 API for Abaqus FEA .odb Files and related Command Line Visualization Tool, with an Additive Manufacturing Focus
 Author-email: Clark Hensley <clarkhensley@duck.com>
 Maintainer-email: Clark Hensley <clarkhensley@duck.com>
 License: MIT License
         
         Copyright (c) 2023 Matthew W. Priddy
```

### Comparing `odb-plotter-0.4.6/src/odb_plotter.egg-info/SOURCES.txt` & `odb-plotter-0.5.0/src/odb_plotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.6/src/odbp/cli.py` & `odb-plotter-0.5.0/src/odbp/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,17 +52,14 @@
 
             elif user_input in cli_options.select_options:
                 select_files(state, user_options)
 
             elif user_input in cli_options.convert_options:
                 convert(state)
 
-            elif user_input in cli_options.seed_options:
-                set_seed_size(state)
-
             elif user_input in cli_options.extrema_options:
                 set_extrema(state)
 
             elif user_input in cli_options.time_options:
                 set_time(state)
 
             elif user_input in cli_options.time_sample_options:
@@ -182,52 +179,36 @@
         user_input: str = input("Please enter the desired name of the generated .hdf5 file: ")
         if confirm(f"You entered {user_input}", "Is this correct", "yes"):
             state.odb_to_hdf(user_input)
             break
 
 
 def pre_process_data(state: OdbVisualizer, user_options: UserOptions):
-    mesh_seed_size: Union[float, None] = None
     meltpoint: Union[float, None] = None
     low_temp: Union[float, None] = None
     time_sample: Union[int, None] = None
 
     if user_options.config_file_path is not None:
         config_file: TextIO
         with open(user_options.config_file_path, "rb") as config_file:
             config: dict[str, Any] = tomllib.load(config_file)
 
         if "hdf_file_path" in config:
             if config["hdf_file_path"] != state.hdf_file_path:
                 print("INFO: File name provided and File Name in the config do not match. This could be an issue, or it might be fine")
 
-        if "mesh_seed_size" in config:
-            mesh_seed_size = config["mesh_seed_size"]
-
         if "meltpoint" in config:
             meltpoint = config["meltpoint"]
 
         if "low_temp" in config:
             low_temp = config["low_temp"]
 
         if "time_sample" in config:
             time_sample = config["time_sample"]
 
-        # Manage mesh_seed_size
-        if mesh_seed_size is not None:
-            print(f"Setting Mesh Seed Size to stored value of {mesh_seed_size}")
-            state.set_mesh_seed_size(mesh_seed_size)
-
-        elif hasattr(state, "mesh_seed_size"):
-            print(f"Setting Default Seed Size of the Mesh to given value of {state.mesh_seed_size}")
-
-        else: # Neither the stored value or the given value exist
-            print("No Mesh Seed Size found. You must set it:")
-            set_seed_size(state)
-
         # Manage meltpoint
         if meltpoint is not None:
             print(f"Setting Melting Point to stored value of {meltpoint}")
             state.set_meltpoint(meltpoint)
 
         elif hasattr(state, "meltpoint"):
             print(f"Setting Default Melting Point to given value of {state.meltpoint}")
@@ -256,19 +237,15 @@
         elif hasattr(state, "time_sample"):
             print(f"Setting Default Time Sample to given value of {state.time_sample}")
 
         else: # Neither the stored value nor the given value exist
             print("No Time Sample found. You must set it:")
             set_time_sample(state)
 
-    if not all((hasattr(state, "mesh_seed_size"), hasattr(state, "meltpoint"), hasattr(state, "low_temp"), hasattr(state, "time_sample"))):
-
-        # here, we need to set at least one of the things
-        if mesh_seed_size is None:
-            set_seed_size(state)
+    if not all(hasattr(state, "meltpoint"), hasattr(state, "low_temp"), hasattr(state, "time_sample")):
 
         if meltpoint is None:
             set_meltpoint(state)
 
         if low_temp is None:
             set_low_temp(state)
 
@@ -415,29 +392,14 @@
             state.set_y_high(y_high)
             state.set_z_low(z_low)
             state.set_z_high(z_high)
             print(f"Spatial Dimensions Updated to:\nX from {state.x.low} to {state.x.high}\nY from {state.y.low} to {state.y.high}\nZ from {state.z.low} to {state.z.high}")
             break
 
 
-def set_seed_size(state: OdbVisualizer) -> None:
-    print("INFO: You must enter the Mesh Seed Size with which the .hdf5 was generated")
-    while True:
-        try:
-            seed: float = float(input("Enter the Default Seed Size of the Mesh: "))
-
-            if confirm(f"Mesh Seed Size: {seed}", "Is this correct", "yes"):
-                state.set_mesh_seed_size(seed)
-                print(f"Mesh Seed Size set to: {state.mesh_seed_size}")
-                break
-
-        except ValueError:
-            print("Error, Default Seed Size must be a number")
-
-
 def set_meltpoint(state: OdbVisualizer) -> None:
     while True:
         try:
             meltpoint = float(input("Enter the meltpoint of the Mesh: "))
 
             if confirm(f"Meltng Point: {meltpoint}", "Is this correct", "yes"):
                 state.set_meltpoint(meltpoint)
```

### Comparing `odb-plotter-0.4.6/src/odbp/data/config.toml` & `odb-plotter-0.5.0/src/odbp/data/config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -102,30 +102,23 @@
 # Not set by default. Enter a value and uncomment to pass a default value
 # meltpoint =
 
 #####
 
 #####
 
-# In general, don't set mesh_seed_size or time_sample with these files
-# If you are creating a .hdf5 file from a .odb,
-# you can pass in the mesh_seed_size in an input file.
 # A default time sample of 1 works, but should almost always be overwritten
 # Otherwise, you should rely on the corresponding config file with the .hdf5
 
 #####
 
 # time sampling interval (N for "extract every Nth frame")
 # Default value of 1, but expect this to almost always be overwritten
 time_sample = 1
 
-# mesh seed size with which the .odb was generated
-# Not set by default. Enter a value and uncomment to pass a default value
-# mesh_seed_size =
-
 #####
 
 # which program to run the abaqus python commands with
 # Defaults to "abaqus" but, for example, if you have both abaqus 2019 and 2022
 # installed, and use abaqus 2019, you would set this to "abq2019"
 abaqus_program = "abaqus"
```

### Comparing `odb-plotter-0.4.6/src/odbp/odb_visualizer.py` & `odb-plotter-0.5.0/src/odbp/odb_visualizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,186 @@
 #!/usr/bin/env python3
 
+"""
+ODBPlotter odb_visualizer.py
+ODBPlotter
+https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
+MIT License (c) 2023
+
+A child class of the ODB class which implements two- and three-dimensional
+plotting capabilities.
+"""
 
-import os
+import operator
+import multiprocessing
 import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.colors as mcolors
 import pyvista as pv
-from typing import TextIO, Union, Any
 from .odb import Odb
-
-
-class MeltpointNotSetError(Exception):
-    def __init__(self) -> None:
-        self.message = "You must enter the meltpoint and, optionally, the string name of a plt colormap (default \"turbo\") in order to set the colormap"
+from .util import DataFrameType, MultiprocessingPoolType
 
 
 class OdbVisualizer(Odb):
     """
-
+    Serves exactly as a normal Odb instance, but includes
+    plotting capabilities
     """
-    def __init__(self) -> None:
-        Odb.__init__(self)
-
-        self.interactive: bool
-
-        self.angle: str
-        self.x_rot: int
-        self.y_rot: int
-        self.z_rot: int
-
-        self.colormap_name: str
-        self.colormap: pv.LookupTable
-
-
-    def select_colormap(self) -> None:
-        if not (hasattr(self, "meltpoint") or hasattr(self, "colormap_name")):
-            raise MeltpointNotSetError
-
-        # TODO different melt color? Don't plot from as low as 0?
-        self.colormap = pv.LookupTable(cmap=self.colormap_name, scalar_range=(self.low_temp, self.meltpoint), above_range_color=(0.75, 0.75, 0.75, 1.0))
-
-
-    # Overload parent's set_meltpoint method to always select colormap
-    def set_meltpoint(self, meltpoint: float) -> None:
-        if not isinstance(meltpoint, float):
-            meltpoint = float(meltpoint)
-        self.meltpoint = meltpoint
-
-        if hasattr(self, "low_temp"):
-            self.select_colormap()
-
 
-    # Overload parent's set_low_temp method to always select colormap
-    def set_low_temp(self, low_temp: float) -> None:
-        if not isinstance(low_temp, float):
-            low_temp = float(low_temp)
-        self.low_temp = low_temp
-
-        if hasattr(self, "meltpoint"):
-            self.select_colormap()
-
-
-    def plot_time_3d(self, time: float, label: str, interactive: bool)-> Any:
-        curr_nodes: Any = self.out_nodes[self.out_nodes["Time"] == time]
-
-        formatted_time: str = format(round(time, 2), ".2f")
-        combined_label = f"{label}-{formatted_time}"
-
-        off_screen: bool = not interactive
-        plotter = pv.Plotter(off_screen=off_screen, window_size=[1920, 1080], lighting="three lights")
-        plotter.add_text(combined_label, position="upper_edge", color="#000000", font="courier", )
-        faces: list[str] = ["x_low", "x_high", "y_low", "y_high", "z_low", "z_high"]
-        face: str
-        for face in faces:
-            selected_nodes: Any
-
-            # TODO This whole idea could be parameterized, but it might be less readable
-            if "x" in face:
-                if "low" in face:
-                    selected_nodes = curr_nodes[curr_nodes["X"] == self.x.low]
-                else: # if "high" in face:
-                    selected_nodes = curr_nodes[curr_nodes["X"] == self.x.high]
-
-            elif "y" in face:
-                if "low" in face:
-                    selected_nodes = curr_nodes[curr_nodes["Y"] == self.y.low]
-                else: # if "high" in face:
-                    selected_nodes = curr_nodes[curr_nodes["Y"] == self.y.high]
-
-            else: # if "z" in face
-                if "low" in face:
-                    selected_nodes = curr_nodes[curr_nodes["Z"] == self.z.low]
-                else: # if "high" in face:
-                    selected_nodes = curr_nodes[curr_nodes["Z"] == self.z.high]
-
-            dims_columns: set[str] = set(["X", "Y", "Z"])
-            points: Any = pv.PolyData(selected_nodes.drop(columns=list(set(selected_nodes.columns.values.tolist()) - dims_columns)).to_numpy())
-            points["Temp"] = selected_nodes["Temp"].to_numpy()
-            surface: Any = points.delaunay_2d()
-
-            # For whatever reason, the input data is rotated 180 degrees about the y axis. This fixes that.
-            #surface = surface.rotate_z(180)
-
-            plotter.add_mesh(surface, scalars="Temp", cmap=self.colormap, scalar_bar_args={"title": "Nodal Temperature (kelvins)", "font_family": "courier", "color": "#000000", "fmt": "%.2f", "position_y": 0})
-            dims_columns: set[str] = set(["X", "Y", "Z"])
-            points: Any = pv.PolyData(selected_nodes.drop(columns=list(set(selected_nodes.columns.values.tolist()) - dims_columns)).to_numpy())
-            points["Temp"] = selected_nodes["Temp"].to_numpy()
-            surface: Any = points.delaunay_2d()
-
-            # For whatever reason, the input data is rotated 180 degrees about the y axis. This fixes that.
-            #surface = surface.rotate_z(180)
-
-        plotter.show_bounds(location="outer", ticks="both", font_size=14.0, font_family="courier", color="#000000", axes_ranges=[self.x.low, self.x.high, self.y.low, self.y.high, self.z.low, self.z.high])
-        plotter.set_background(color="#FFFFFF")
-
-        #plotter.camera.focal_point = ((self.x.high + self.x.low)/2, (self.y.high + self.y.low)/2, (self.z.high + self.z.low)/2)
-        plotter.camera.elevation = 0
-        plotter.camera.azimuth = 270
-        plotter.camera.roll = 300
-        plotter.camera_set = True
-        #plotter.disable_shadows()
-        #plotter.add_light(pv.Light(light_type="headlight"))
+    __slots__ = (
+        "_interactive",
+        "_angle",
+        "_colormap"
+        )
+    def __init__(self) -> None:
+        """
+        """
+        
+        super().__init__()
+
+        self._interactive: bool = False
+        self._colormap: str = "turbo"
+
+        # TODO ???
+        self._angle: str | tuple[float, float, float]
+
+
+    @property
+    def colormap(self) -> str:
+        return self._colormap
+    
+
+    @colormap.setter
+    def colormap(self, value: str) -> None:
+        self._colormap = value
+
+
+    @property
+    def interactive(self) -> bool:
+        return self._interactive
+
+
+    @interactive.setter
+    def interactive(self, value: bool) -> None:
+        self._interactive = value
+
+
+    def plot_3d_all_times(self, label: str = "") -> list[pv.Plotter]:
+        """
+        """
+
+        times: DataFrameType = np.sort(self._filtered_nodes["Time"].unique())
+        
+        plotting_args: list[
+            tuple[
+                float,
+                str
+                ]
+            ] = [(time, label) for time in times]
+        results: list[pv.Plotter] = list()
+        time: float
+        for time in times:
+            results.append(self.plot_3d_single(time, label))
+        # TODO Any way to make this work?
+        """
+        # TODO dataclass
+        plotting_args: list[
+            tuple[
+                float,
+                str
+                ]
+            ] = [(time, label) for time in times]
+        results: list[pv.Plotter] = list()
+        pool: MultiprocessingPoolType
+        with multiprocessing.Pool() as pool:
+            results: list[pv.Plotter] = pool.starmap(
+                self.plot_3d_single,
+                plotting_args
+                )"""
+
+        return results 
+
+
+    def plot_3d_single(
+        self,
+        time: float,
+        label: str
+        )-> pv.Plotter | None:
+        """
+        """
+
+        dims_columns: set[str] = {"X", "Y", "Z"}
+        combined_label: str = f"{label}-{round(time, 2):.2f}"
+
+        plotter: pv.Plotter = pv.Plotter(
+            off_screen=(not self._interactive),
+            window_size=(1920, 1080),
+            lighting="three lights"
+            )
+
+        plotter.add_text(
+            combined_label,
+            position="upper_edge",
+            color="#000000",
+            font="courier"
+        )
+
+        instance_nodes: DataFrameType = self.filter_nodes(
+            "Time",
+            time,
+            operator.eq
+        )
+
+        if not instance_nodes.empty:
+            points: pv.PolyData = pv.PolyData(
+                instance_nodes.drop(
+                    columns=list(
+                        set(self._target_nodes.columns.values.tolist())
+                        - dims_columns
+                        )
+                    ).to_numpy()
+                )
+            
+            points["Temp"] = instance_nodes["Temp"].to_numpy()
+            mesh: pv.PolyData = points.delaunay_3d()
+
+            plotter.add_mesh(
+                mesh,
+                scalars="Temp",
+                cmap = pv.LookupTable(
+                    cmap=self._colormap,
+                    scalar_range=(
+                        self._temp_low,
+                        self._temp_high
+                        ),
+                    above_range_color=(
+                        0.75,
+                        0.75,
+                        0.75,
+                        1.0
+                    )
+                ),
+                scalar_bar_args={
+                    "title": "Nodal Temperature (Kelvin)",
+                    "font_family": "courier",
+                    "color": "#000000",
+                    "fmt": "%.2f",
+                    "position_y": 0
+                }
+            )
+
+            plotter.show_bounds(
+                location="outer",
+                ticks="both",
+                font_size=14.0,
+                font_family="courier",
+                color="#000000",
+                axes_ranges=points.bounds
+                )
+
+            plotter.set_background(color="#FFFFFF")
+
+            # TODO
+            plotter.camera.elevation = 0
+            plotter.camera.azimuth = 270
+            plotter.camera.roll = 300
+            plotter.camera_set = True
 
-        return plotter
+            return plotter
```

### Comparing `odb-plotter-0.4.6/src/odbp/py2_scripts/extract.py` & `odb-plotter-0.5.0/src/odbp/py2_scripts/extract.py`

 * *Files identical despite different names*

### Comparing `odb-plotter-0.4.6/src/odbp/py2_scripts/odb_to_npz.py` & `odb-plotter-0.5.0/src/odbp/py2_scripts/odb_to_npz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,234 +1,238 @@
-# Author: CJ Nguyen
-# Heavily based off of example ODB extraction script from the CMML Github written by Will Furr and Matthew Dantin
-# This script takes an ODB and converts the nodeset data to npz files
-# The data that is created is the following
-# * npzs containing temperatures for each node at every frame, one dataframe per step of the program
-# * npz containing coordinate data for each node, organized by nodelabel - xyz coordinate
-# * npz containing the starting time of each frame
-
-# Usage: python <script name> <odb file name> <inp file name>
-# Where <inp file name> is the .inp file used to generate the ODB (needed for the timing of each frame)
-# NOTE: This script makes three major assumptions:
-# * The Odb has a part named "PART-1-1"
-# * The part's first nodeset is the nodeset that references all nodes
-# * The first frame of the sequence outputs the coordinates of all nodes
-# Without these assumptions, the script will have unexpected behavior.
+#!/usr/bin/env python
+
+"""
+ODBPlotter odb_to_npz.py
+
+ODBPlotter
+https://www.github.com/Computational-Mechanics-Materials-Lab/ODBPlotter
+MIT License (c) 2023
+
+This is a Python 2 file which implements an Abaqus Python interface to
+convert data from within a .odb file into a hierarchical directory of .npz
+compressed numpy arrays. This is used to translate .odb data from the Python 2
+environment to a modern Python 3 environment
+
+Originally authored by CMML member CJ Nguyen, based before on extraction
+script written by CMML members Will Furr and Matt Dantin
+"""
 
-# This script can be configured by having a file of name `odb_to_npz_config.json` in the working directory.
-# The format of this file is specified in the readme.
 
 import os
-from odbAccess import openOdb, version
-from abaqusConstants import *
+import pickle
 import numpy as np
 import argparse
-from multiprocessing import Process
+import multiprocessing
+from odbAccess import openOdb
+
+
+def main():
+    """
+    Helper function to parse command-line arguments from subprocess.run
+    and format these values to correctly convert the .odb to the .npz files.
+    This reads the pickle file passed by file path and passes these values
+    to the convert_odb_to_npz() method
+    """
+
+    # Parse the subprocess input args
+    input_args = "input args"
+    parser = argparse.ArgumentParser()
+    parser.add_argument(input_args, nargs="*")
+    odb_path, pickle_path, result_path = vars(parser.parse_args())[input_args]
 
+    # Try our best to manage Python 2 file handling
+    pickle_file = open(pickle_path, "rb")
+    try:
+        data_to_extract = pickle.load(pickle_file)
 
-def main(odb_path, frame_step, nodeset):
+    finally:
+        pickle_file.close()
 
+    # Now we can remove the file
+    os.remove(pickle_path)
+
+    nodesets = data_to_extract["nodesets"]
+    frames = data_to_extract["frames"]
+
+    result_name = convert_odb_to_npz(odb_path, nodesets, frames)
+    result_file = open(result_path, "wb")
+    try:
+        pickle.dump(result_name, result_file)
+    finally:
+        result_file.close()
+
+
+
+def convert_odb_to_npz(odb_path, nodesets, frames):
+    """
+    Based on the 4 lists given, convert the .odb data to .npz files
+    odb_path: str path to the .odb file
+    nodes: list[int] which nodes to convert (default to all)
+    parts: list[str] which parts to convert (default to no specific part)
+    nodesets: list[str] which nodesets to convert (default to the first
+    nodeset)
+    frames: list[int] which frames to convert (default to all)
+
+    return the name of the directory of .npz files created
+    """
+
+    # Create the results directory
     parent_dir = os.path.join(os.getcwd(), "tmp_npz")
     if not os.path.exists(parent_dir):
         os.mkdir(parent_dir)
 
-    #for part in parts:
-    # Create directory to store npzs
-    coord_file = os.path.join(parent_dir, "node_coords.npz")
-
     temps_dir = os.path.join(parent_dir, "temps")
     if not os.path.exists(temps_dir):
         os.mkdir(temps_dir)
 
     time_dir = os.path.join(parent_dir, "step_frame_times")
     if not os.path.exists(time_dir):
         os.mkdir(time_dir)
 
     odb = openOdb(odb_path, readOnly=True)
 
     steps = odb.steps
 
-    base_times = [(step_key, step_val.totalTime) for step_key, step_val in steps.items()]
+    base_times = [
+        (step_key, step_val.totalTime) for step_key, step_val in steps.items()
+        ]
     
     assembly = odb.rootAssembly
     nodeset_keys = assembly.nodeSets.keys()
-    if nodeset not in nodeset_keys:
-        raise ValueError("'{0}' is not a valid nodeset key. Possible values in this .odb are {1}".format(nodeset, nodeset_keys))
+    if nodesets is None:
+        nodesets = nodeset_keys
+    else:
+        for nodeset in nodesets:
+            if nodeset not in nodeset_keys:
+                raise ValueError(
+                    '"{0}" is not a valid nodeset key.' \
+                        'Possible values in this .odb are "{1}"'
+                .format(nodeset, nodeset_keys)
+                )
 
     odb.close()
 
-    if version == str(2022):
-        read_coords_procs = list()
-        for step_key, _ in base_times:
-            p = Process(target=read_frame_coords, args=(step_key, filename, frame_step, coord_file, nodeset))
-            p.start()
-            read_coords_procs.append(p)
+    for nodeset in nodesets:
+        for step_key, base_time in base_times:
+            coord_file = os.path.join(parent_dir, "node_coords.npz")
+            read_nodeset_coords(odb_path, nodeset, coord_file, step_key)
+            read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset)
 
-        for p in read_coords_procs:
-            p.join()
+    return parent_dir
 
 
-        read_step_procs = list()
-        for step_key, base_time in base_times:
-            p = Process(target=read_step_data, args=(temps_dir, time_dir, step_key, base_time, frame_step, filename, nodeset))
-            p.start()
-            read_step_procs.append(p)
+def read_step_data(odb_path, temps_dir, time_dir, step_key, base_time, frames, nodeset):
+    odb = openOdb(odb_path, readOnly=True)
+    steps = odb.steps
 
-        for p in read_step_procs:
-            p.join()
-            
-        """elif version == str(2019):
-        read_coords_procs = list()
-        for step_key, _ in base_times:
-            p = Process(target=read_frame_coords2019, args=(step_key, filename, frame_step, coord_file, nodeset))
-            p.start()
-            read_coords_procs.append(p)
-            
-        for p in read_coords_procs:
-            p.join()
+    curr_step_dir = os.path.join(temps_dir, step_key)
+    if not os.path.exists(curr_step_dir):
+        os.mkdir(curr_step_dir)
+
+    if frames is not None:
+        max_frame = max(frames)
 
-        read_step_procs = list()
-        for step_key, base_time in base_times:
-            p = Process(target=read_step_data2019, args=(temps_dir, time_dir, step_key, base_time, frame_step, filename, nodeset))
-            p.start()
-            read_step_procs.append(p)
-            
-        for p in read_step_procs:
-            p.join()"""
-            
     else:
-        print("Unsupported Abaqus Version")
+        max_frame = len(steps[step_key].frames)
 
+    max_pad = len(str(max_frame))
 
-def read_nodeset_items(nodeset_dir, nodeset_name, filename, part):
-    odb = openOdb(filename, readOnly=True)
-    assembly = odb.rootAssembly
-    nodesets = assembly.instances[part].nodeSets # returns a dictionary of ODB objects
-    out_nodeset_name = os.path.join(nodeset_dir, nodeset_name)
-    out_nodeset_name += ".npz"
-    np.savez_compressed(out_nodeset_name, np.array([node.label for node in nodesets[nodeset_name].nodes]))
-    odb.close()
+    manager = multiprocessing.Manager()
+    frame_times = manager.list()
+    #frame_times = list()
+    if len(steps[step_key].frames) > 0:
+        idx_list = [i for i in range(len(steps[step_key].frames))]
+        idx_list_len = len(idx_list)
+        idx_list_max = idx_list[-1]
+        num_cpus = multiprocessing.cpu_count()
+        # TODO: what if the length isn't divisible by the number of processors (is it now?)
+        final_idx_list = [idx_list[i: i + int(idx_list_len / num_cpus)] for i in range(0, idx_list_len, max(int(idx_list_len / num_cpus), 1))]
+        odb.close()
+
+        temp_procs = list()
+        for idx_list in final_idx_list:
+            p = multiprocessing.Process(target=read_single_frame_temp, args=(odb_path, idx_list, max_pad, frames, step_key, curr_step_dir, frame_times, base_time, nodeset))
+            p.start()
+            temp_procs.append(p)
+
+        for p in temp_procs:
+            p.join()
+
+        np.savez_compressed(
+            "{}.npz".format(
+                os.path.join(
+                    time_dir,
+                    step_key
+                    )
+                ),
+            np.sort(
+                np.array(
+                    frame_times
+                    )
+                )
+            )
 
 
-def read_step_data(temps_dir, time_dir, step_name, base_time, frame_step, filename, nodeset):
+def read_single_frame_temp(odb_path, idx_list, max_pad, frames, step_key, curr_step_dir, frame_times, base_time, nodeset):
 
-    odb = openOdb(filename, readOnly=True)
+    odb = openOdb(odb_path, readOnly=True)
     steps = odb.steps
     assembly = odb.rootAssembly
 
-    curr_step_dir = os.path.join(temps_dir, step_name)
-    if not os.path.exists(curr_step_dir):
-        os.mkdir(curr_step_dir)
+    for idx in idx_list:
+        if frames is not None and idx not in frames:
+            continue
+        
+        frame = steps[step_key].frames[idx]
 
-    frame_times = list()
-    step_size = len(steps[step_name].frames)
-    for num in range(0, step_size, frame_step):
-        frame_pct = ((num + 1) * 100) / step_size
-        print("\tGetting node temperatures for frame {0}, {1}% Complete".format(num, frame_pct))
-        frame = steps[step_name].frames[num]
-        field = frame.fieldOutputs['NT11'].getSubset(region=assembly.nodeSets[nodeset])
+        field = frame.fieldOutputs["NT11"].getSubset(region=assembly.nodeSets[nodeset])
         frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
         node_temps = list()
         for item in field.values:
-            # e.g. for node in values
             temp = item.data
             node_temps.append(temp)
-        np.savez_compressed(os.path.join(curr_step_dir, "frame_{}".format(num)), np.array(node_temps))
-    np.savez_compressed("{}.npz".format(os.path.join(time_dir, step_name)), np.array(frame_times))
 
-    odb.close()
+        num = str(idx + 1).zfill(max_pad)
+        np.savez_compressed(
+                os.path.join(
+                    curr_step_dir,
+                    "frame_{".format(num)
+                    ),
+                np.array(node_temps)
+                )
 
+    odb.close()
 
-def read_frame_coords(step_key, filename, frame_step, coord_file, nodeset):
-    odb = openOdb(filename, readOnly=True)
-    steps = odb.steps
-    assembly = odb.rootAssembly
-    #nodesets = assembly.instances[config["first_part"]].nodeSets # returns a dictionary of ODB objects
-    frame_list = steps[step_key].frames
-    frame_size = len(frame_list)
-    for num in range(0, frame_size, frame_step):
-        frame = frame_list[num]
-        # The below reference pulls from the nodeset representing all nodes
-        coords = frame.fieldOutputs['COORD'].getSubset(region=assembly.nodeSets[nodeset])
-        frame_pct = ((num + 1) * 100) / frame_size
-        print("\tGetting node coordinates for frame {0}, {1}% Complete".format(num, frame_pct))
-
-        coord_arr = list()
-        for item in coords.values:
-            node = item.nodeLabel
-            coord = item.data
-            xyz = [node]
-            for axis in coord:
-                xyz.append(axis)
-            coord_arr.append(xyz)
-        np.savez_compressed(coord_file, np.array(coord_arr))
 
-    odb.close()
+def read_nodeset_coords(odb_path, nodeset, coord_file, step_key):
 
+    # Only extract coordinates from the first given nodeset/step
+    if not os.path.exists(coord_file):
 
-"""def read_frame_coords2019(step_key, filename, frame_step, coord_file, nodeset):
-    odb = openOdb(filename, readOnly=True)
-    steps = odb.steps
-    assembly = odb.rootAssembly
-    #nodesets = assembly.instances[config["first_part"]].nodeSets # returns a dictionary of ODB objects
-    frame_list = steps[step_key].frames
-    frame_size = len(frame_list)
-    print(frame_size)
-    for num in range(0, frame_size, frame_step):
-        frame = frame_list[num]
-        # The below reference pulls from the nodeset representing all nodes
-        coords = frame.fieldOutputs['COORD'].getSubset(region=assembly.nodeSets[nodeset])
-        frame_pct = ((num + 1) * 100) / frame_size
-        print("\tGetting node coordinates for frame {0}, {1}% Complete".format(num, frame_pct))
-
-        coord_arr = list()
-        for item in coords.values:
-            node = item.nodeLabel
-            coord = item.data
-            xyz = [node]
-            for axis in coord:
-                xyz.append(axis)
-            coord_arr.append(xyz)
-        np.savez(coord_file, np.array(coord_arr))
+        odb = openOdb(odb_path, readOnly=True)
+        assembly = odb.rootAssembly
+        steps = odb.steps
 
-    odb.close()"""
-    
-    
-"""def read_step_data2019(temps_dir, time_dir, step_name, base_time, frame_step, filename, nodeset):
+        frame = steps[step_key].frames[0]
 
-    odb = openOdb(filename, readOnly=True)
-    steps = odb.steps
-    assembly = odb.rootAssembly
+        try:
+            coords = frame.fieldOutputs["COORD"].getSubset(region=assembly.nodeSets[nodeset])
 
-    curr_step_dir = os.path.join(temps_dir, step_name)
-    if not os.path.exists(curr_step_dir):
-        os.mkdir(curr_step_dir)
+            results_list = list()
+            for item in coords.values:
+                node = item.nodeLabel
+                coord = item.data
+                xyz = [node]
+                for axis in coord:
+                    xyz.append(axis)
+                results_list.append(xyz)
 
-    frame_times = list()
-    step_size = len(steps[step_name].frames)
-    for num in range(0, step_size, frame_step):
-        frame_pct = ((num + 1) * 100) / step_size
-        print("\tGetting node temperatures for frame {0}, {1}% Complete".format(num, frame_pct))
-        frame = steps[step_name].frames[num]
-        field = frame.fieldOutputs['NT11'].getSubset(region=assembly.nodeSets[nodeset])
-        frame_times.append(float(format(round(frame.frameValue + base_time, 5), ".2f")))
-        node_temps = list()
-        for item in field.values:
-            # e.g. for node in values
-            temp = item.data
-            node_temps.append(temp)
+            np.savez_compressed(coord_file, np.array(results_list))
 
-        np.savez(os.path.join(curr_step_dir, "frame_{}".format(num)), np.array(node_temps))
+        except KeyError:
+            pass
 
-    np.savez("{}.npz".format(os.path.join(time_dir, step_name)), np.array(frame_times))
+        odb.close()
 
-    odb.close()"""
-    
     
 if __name__ == "__main__":
-    input_args = "input args"
-    parser = argparse.ArgumentParser()
-    parser.add_argument(input_args, nargs="*")
-    filename, frame_step, nodeset = vars(parser.parse_args())[input_args]
-    frame_step = int(frame_step)
-
-    main(filename, frame_step, nodeset)
+    main()
```

### Comparing `odb-plotter-0.4.6/src/odbp/state.py` & `odb-plotter-0.5.0/src/odbp/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,18 +52,14 @@
         self.select_help: str = "Select a .hdf5 file or a .odb file"
         self.select_options_formatted: str = ", ".join(self.select_options)
 
         self.convert_options: list[str] = ["convert"]
         self.convert_help: str = "Convert a selected .odb file to a .hdf5 file"
         self.convert_options_formatted: str = ", ".join(self.convert_options)
 
-        self.seed_options: list[str] = ["seed", "mesh"]
-        self.seed_help: str = "Set the Mesh Seed Size"
-        self.seed_options_formatted: str = ", ".join(self.seed_options)
-
         self.extrema_options: list[str] = ["extrema", "range"]
         self.extrema_help: str = "Set the upper and lower x, y, and z bounds for plotting"
         self.extrema_options_formatted: str = ", ".join(self.extrema_options)
 
         self.time_options: list[str] = ["time"]
         self.time_help: str = "Set the upper and lower time bounds"
         self.time_options_formatted: str = ", ".join(self.time_options)
@@ -120,15 +116,14 @@
         self.help_help: str = "Show this menu"
         self.help_options_formatted: str = ", ".join(self.help_options)
 
         self.longest_len: int = max(
                 len(self.quit_options_formatted),
                 len(self.select_options_formatted),
                 len(self.convert_options_formatted),
-                len(self.seed_options_formatted),
                 len(self.extrema_options_formatted),
                 len(self.time_options_formatted),
                 len(self.time_sample_options_formatted),
                 len(self.meltpoint_options_formatted),
                 len(self.low_temp_options_formatted),
                 len(self.title_label_options_formatted),
                 len(self.directory_options_formatted),
@@ -142,15 +137,14 @@
     def print_help(self) -> None:
         print(
     f"""ODBPlotter Help:
 {self.help_options_formatted.ljust(self.longest_len)} -- {self.help_help}
 {self.quit_options_formatted.ljust(self.longest_len) } -- {self.quit_help}
 {self.select_options_formatted.ljust(self.longest_len)} -- {self.select_help}
 {self.convert_options_formatted.ljust(self.longest_len)} -- {self.convert_help}
-{self.seed_options_formatted.ljust(self.longest_len)} -- {self.seed_help}
 {self.extrema_options_formatted.ljust(self.longest_len)} -- {self.extrema_help}
 {self.time_options_formatted.ljust(self.longest_len)} -- {self.time_help}
 {self.time_sample_options_formatted.ljust(self.longest_len)} -- {self.time_sample_help}
 {self.meltpoint_options_formatted.ljust(self.longest_len)} -- {self.meltpoint_help}
 {self.low_temp_options_formatted.ljust(self.longest_len)} -- {self.low_temp_help}
 {self.title_label_options_formatted.ljust(self.longest_len)} -- {self.title_label_help}
 {self.directory_options_formatted.ljust(self.longest_len)} -- {self.directory_help}
@@ -179,15 +173,14 @@
             "X Range": f"{state.x.low if hasattr(state.x, 'low') else 'not set'} to {state.x.high if hasattr(state.x, 'high') else 'not set'}",
             "Y Range": f"{state.y.low if hasattr(state.y, 'low') else 'not set'} to {state.y.high if hasattr(state.y, 'high') else 'not set'}",
             "Z Range": f"{state.z.low if hasattr(state.z, 'low') else 'not set'} to {state.z.high if hasattr(state.z, 'high') else 'not set'}",
             "Time Range": f"{state.time_low if hasattr(state, 'time_low') else 'not set'} to {state.time_high if hasattr(state, 'time_high') else 'not set'}",
             "Temperature Range": f"{state.low_temp if hasattr(state, 'low_temp') else 'not set'} to {state.meltpoint if hasattr(state, 'meltpoint') else 'not set'}",
         },
         {
-            "Seed Size of the Mesh": f"{state.mesh_seed_size if hasattr(state, 'mesh_seed_size') else 'not set'}",
             "Time Sample of the Mesh": f"{state.time_sample if hasattr(state, 'time_sample') else 'not set'}",
         },
         {
             "Is each time-step being shown in the PyVista interactive Viewer": f"{'Yes' if state.interactive else 'No'}",
             "View Angle": f"{state.angle if hasattr(state, 'angle') else 'not set'}",
             "Rotation around the X Axis": f"{state.elev if hasattr(state, 'elev') else 'not set'}",
             "Rotation around the Y Axis": f"{state.azim if hasattr(state, 'azim') else 'not set'}",
@@ -243,15 +236,14 @@
     parser.add_argument("-s", "--hdf-source-directory", help="Directory from which to source .hdf5 files")
     parser.add_argument("-b", "--odb-source-directory", help="Directory from which to source .odb files")
     parser.add_argument("-r", "--results-directory", help="Directory in which to store results")
 
     parser.add_argument("-o", "--odb", help="Path to the desired .odb file")
     parser.add_argument("-m", "--meltpoint", help="Melting Point of the Mesh")
     parser.add_argument("-l", "--low-temp", help="Temperature lower bound, defaults to 300 K")
-    parser.add_argument("-S", "--mesh-seed-size", help="Mesh seed size of the .odb file")
     parser.add_argument("-t", "--time-sample", help="Time-sample value (N for every Nth frame you extracted). Defaults to 1")
 
     parser.add_argument("-H", "--hdf", help="Path to desired .hdf5 file")
 
     parser.add_argument("-T", "--title", help="Title to save each generated file under")
     parser.add_argument("-L", "--label", help="Label to put on each generated image")
 
@@ -460,17 +452,14 @@
 
         if "meltpoint" in settings_dict:
             state.set_meltpoint(settings_dict["meltpoint"])
 
         if "low_temp" in settings_dict:
             state.set_low_temp(settings_dict["low_temp"])
 
-        if "mesh_seed_size" in settings_dict:
-            state.set_mesh_seed_size(settings_dict["mesh_seed_size"])
-
         if "time_sample" in settings_dict:
             state.set_time_sample(settings_dict["time_sample"])
 
         if "hdf" in settings_dict:
             state.hdf_file_path = os.path.join(user_options.hdf_source_directory, settings_dict["hdf"])
 
     elif "hdf" in settings_dict:
@@ -482,15 +471,14 @@
             sys.exit(1)
 
         else:
             user_options = output
 
         # If none of these values are set, read as many as are available out of the .toml config file
         # Otherwise, the file must have already been read
-        # if not hasattr(state, "meltpoint") and not hasattr(state, "low_temp") and not hasattr(state, "mesh_seed_size") and not hasattr(state, "time_sample"):
 
         # Search for the stored toml values for this hdf
         config: Union[dict[str, Any], None] = None
         if user_options.config_file_path is None:
             print(f".toml config file for {state.hdf_file_path} could not be found")
         else:
             config_file: TextIO
@@ -503,35 +491,27 @@
             state.set_meltpoint(settings_dict["meltpoint"])
 
         if config is not None and "low_temp" in config:
             state.set_low_temp(config["low_temp"])
         elif "low_temp" in settings_dict:
             state.set_low_temp(settings_dict["low_temp"])
 
-        if config is not None and "mesh_seed_size" in config:
-            state.set_mesh_seed_size(config["mesh_seed_size"])
-        elif "mesh_seed_size" in settings_dict:
-            state.set_mesh_seed_size(settings_dict["mesh_seed_size"])
-
         if config is not None and "time_sample" in config:
             state.set_time_sample(config["time_sample"])
         elif "time_sample" in settings_dict:
             state.set_time_sample(settings_dict["time_sample"])
 
     else: # The case where a .odb file and a .hdf5 file were not provided
 
         if "meltpoint" in settings_dict:
             state.set_meltpoint(settings_dict["meltpoint"])
 
         if "low_temp" in settings_dict:
             state.set_low_temp(settings_dict["low_temp"])
 
-        if "mesh_seed_size" in settings_dict:
-            state.set_mesh_seed_size(settings_dict["mesh_seed_size"])
-
         if "time_sample" in settings_dict:
             state.set_time_sample(settings_dict["time_sample"])
 
     # The 4 dimensions and the two booleans are always set here if they exist
     # The 5th dimension, temperature, is not set here because it shouldn't
     # change based on the file, even if the spatial
     # or temporal dimensions change
```

