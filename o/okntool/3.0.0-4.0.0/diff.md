# Comparing `tmp/okntool-3.0.0.tar.gz` & `tmp/okntool-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-3.0.0.tar", last modified: Sun May 21 23:05:28 2023, max compression
+gzip compressed data, was "okntool-4.0.0.tar", last modified: Thu Jun  1 08:24:33 2023, max compression
```

## Comparing `okntool-3.0.0.tar` & `okntool-4.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.780034 okntool-3.0.0/
--rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      555 2023-05-21 23:05:28.780034 okntool-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.770061 okntool-3.0.0/okntool/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-3.0.0/okntool/__init__.py
--rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-3.0.0/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0    77412 2023-05-21 23:00:52.000000 okntool-3.0.0/okntool/okntool.py
-drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.779037 okntool-3.0.0/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 23:05:09.000000 okntool-3.0.0/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 23:05:28.780034 okntool-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-05-21 22:34:58.000000 okntool-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.189015 okntool-4.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:24:33.187587 okntool-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.180604 okntool-4.0.0/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.0/okntool/__init__.py
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.0/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0   102106 2023-06-01 08:13:39.000000 okntool-4.0.0/okntool/okntool.py
+-rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.0/okntool/simpler_plot_config.json
+drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.187587 okntool-4.0.0/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 08:24:17.000000 okntool-4.0.0/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:24:33.189015 okntool-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-05-31 03:13:16.000000 okntool-4.0.0/setup.py
```

### Comparing `okntool-3.0.0/LICENSE` & `okntool-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-3.0.0/PKG-INFO` & `okntool-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 3.0.0
+Version: 4.0.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-3.0.0/README.md` & `okntool-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `okntool-3.0.0/okntool/oknserver_graph_plot_config.json` & `okntool-4.0.0/okntool/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-3.0.0/okntool/okntool.py` & `okntool-4.0.0/okntool/okntool.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import argparse
 import json
 import csv
 import numpy as np
 import matplotlib.pyplot as plt
 import os
-import pkg_resources
+import importlib.resources as config_resources
 from matplotlib.lines import Line2D
 
 logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
                       "no logMAR", "right_down", "right_up", "left_down", "left_up"]
 
 
 # This function is to get header position from the given array
@@ -232,18 +232,23 @@
     qp_line_thickness = plot_info_input["qp_line_thickness"]
     summary_csv_name = plot_info_input["summary_csv_name"]
     folder_array = get_folder_name_from_dir(data_dir, "trial_id", "disk_condition", summary_csv_name)
 
     adjustment_type = axis_adjustment_types[str(axis_adjustment_type_number)]
     if adjustment_type == "mean_offset":
         plot_info_array = []
-        x_adjust_limit, y_adjust_limit = get_adjust_limit(data_dir, x_data_column_name, y_data_column_name,
-                                                          folder_array, x_axis_limit, y_axis_limit, mean_offset,
-                                                          axis_adjustment_types, axis_adjustment_type_number)
+        x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, None,
+                                                                               x_data_column_name, y_data_column_name,
+                                                                               folder_array, x_axis_limit,
+                                                                               y_axis_limit, mean_offset,
+                                                                               axis_adjustment_types,
+                                                                               axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        if ignore_folder_array:
+            folder_array = [folder for folder in folder_array if folder not in ignore_folder_array]
         for folder_name in folder_array:
             trial_id, disk_condition = str(folder_name).split("_", 1)
             data_dir_to_be_used = os.path.join(data_dir, folder_name, f"updated_{folder_name}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_data_column_name)
             y_array = get_data_array(data_dir_to_be_used, y_data_column_name)
             y_mean = np.nanmean(y_array)
             y_array = [value - y_mean for value in y_array]
@@ -256,18 +261,23 @@
                          "sp_array": sp_array, "qp_array": qp_array,
                          "sp_line_color": sp_line_color, "sp_line_thickness": sp_line_thickness,
                          "qp_line_color": qp_line_color, "qp_line_thickness": qp_line_thickness,
                          "logmar": disk_to_logmar(disk_condition)}
             plot_info_array.append(plot_info)
     else:
         plot_info_array = []
-        x_adjust_limit, y_adjust_limit = get_adjust_limit(data_dir, x_data_column_name, y_data_column_name,
-                                                          folder_array, x_axis_limit, y_axis_limit, mean_offset,
-                                                          axis_adjustment_types, axis_adjustment_type_number)
+        x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, None,
+                                                                               x_data_column_name, y_data_column_name,
+                                                                               folder_array, x_axis_limit,
+                                                                               y_axis_limit, mean_offset,
+                                                                               axis_adjustment_types,
+                                                                               axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        if ignore_folder_array:
+            folder_array = [folder for folder in folder_array if folder not in ignore_folder_array]
         for folder_name in folder_array:
             trial_id, disk_condition = str(folder_name).split("_", 1)
             data_dir_to_be_used = os.path.join(data_dir, folder_name, f"updated_{folder_name}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_data_column_name)
             y_array = get_data_array(data_dir_to_be_used, y_data_column_name)
             signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_folder_name, signal_csv_name)
             sp_array, qp_array = get_sp_and_qp_array(signal_csv_dir, sp_column_name, qp_column_name,
@@ -1186,85 +1196,108 @@
     plt.close()
     print(f"Staircase/progress plot has been saved at:{out_image_dir}")
 
 
 # This function is to produce x and y adjustment limits according the type of adjustment
 # Type comes into the function as int number and is converted into string to be used
 # to retrieve the string type from adjustment dictionary
-def get_adjust_limit(data_dir_input, x_header_input, y_header_input, folder_array_input,
+def get_adjust_limit(data_dir_input, csv_name, x_header_input, y_header_input, folder_array_input,
                      x_axis_limit_input, y_axis_limit_input, mean_offset_input,
                      axis_adjustment_types_input, axis_adjustment_type_number_input):
     adjustment_type = axis_adjustment_types_input[str(axis_adjustment_type_number_input)]
+    ignore_folder_array = []
     print(f"axis_adjustment_type:{adjustment_type}")
     if adjustment_type == "manual":
         x_adjust_limit = {"lower_limit": x_axis_limit_input[0], "upper_limit": x_axis_limit_input[1]}
         y_adjust_limit = {"lower_limit": y_axis_limit_input[0], "upper_limit": y_axis_limit_input[1]}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     elif adjustment_type == "min_max_mean":
         x_lower_limit_array = []
         x_upper_limit_array = []
         y_lower_limit_array = []
         y_upper_limit_array = []
         for folder in folder_array_input:
-            data_dir_to_be_used = os.path.join(data_dir_input, folder, f"updated_{folder}.csv")
-            x_array = get_data_array(data_dir_to_be_used, x_header_input)
-            x_lower_limit_array.append(min(x_array))
-            x_upper_limit_array.append(max(x_array))
-            y_array = get_data_array(data_dir_to_be_used, y_header_input)
-            y_lower_limit_array.append(min(y_array))
-            y_upper_limit_array.append(max(y_array))
+            if not csv_name:
+                csv_name = f"updated_{folder}.csv"
+            try:
+                data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
+                x_array = get_data_array(data_dir_to_be_used, x_header_input)
+                x_lower_limit_array.append(min(x_array))
+                x_upper_limit_array.append(max(x_array))
+                y_array = get_data_array(data_dir_to_be_used, y_header_input)
+                y_lower_limit_array.append(min(y_array))
+                y_upper_limit_array.append(max(y_array))
+            except ValueError:
+                ignore_folder_array.append(folder)
 
         x_adjust_limit = {"lower_limit": int(min(x_lower_limit_array)),
                           "upper_limit": int(max(x_upper_limit_array))}
         y_adjust_limit = {"lower_limit": round(np.nanmean(y_lower_limit_array), 2),
                           "upper_limit": round(np.nanmean(y_upper_limit_array), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     elif adjustment_type == "mean_offset":
         x_lower_limit_array = []
         x_upper_limit_array = []
         for folder in folder_array_input:
-            data_dir_to_be_used = os.path.join(data_dir_input, folder, f"updated_{folder}.csv")
-            x_array = get_data_array(data_dir_to_be_used, x_header_input)
-            x_lower_limit_array.append(min(x_array))
-            x_upper_limit_array.append(max(x_array))
-            y_array = get_data_array(data_dir_to_be_used, y_header_input)
+            if not csv_name:
+                csv_name = f"updated_{folder}.csv"
+            try:
+                data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
+                x_array = get_data_array(data_dir_to_be_used, x_header_input)
+                # print(data_dir_to_be_used)
+                x_lower_limit_array.append(min(x_array))
+                x_upper_limit_array.append(max(x_array))
+                y_array = get_data_array(data_dir_to_be_used, y_header_input)
+            except ValueError:
+                ignore_folder_array.append(folder)
 
         x_adjust_limit = {"lower_limit": int(min(x_lower_limit_array)),
                           "upper_limit": int(max(x_upper_limit_array))}
         y_adjust_limit = {"lower_limit": round(float(- mean_offset_input), 2),
                           "upper_limit": round(float(mean_offset_input), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     else:
         x_lower_limit_array = []
         x_upper_limit_array = []
         y_lower_limit_array = []
         y_upper_limit_array = []
         for folder in folder_array_input:
-            data_dir_to_be_used = os.path.join(data_dir_input, folder, f"updated_{folder}.csv")
-            x_array = get_data_array(data_dir_to_be_used, x_header_input)
-            x_lower_limit_array.append(min(x_array))
-            x_upper_limit_array.append(max(x_array))
-            y_array = get_data_array(data_dir_to_be_used, y_header_input)
-            y_lower_limit_array.append(min(y_array))
-            y_upper_limit_array.append(max(y_array))
+            if not csv_name:
+                csv_name = f"updated_{folder}.csv"
+            try:
+                data_dir_to_be_used = os.path.join(data_dir_input, folder, csv_name)
+                x_array = get_data_array(data_dir_to_be_used, x_header_input)
+                x_lower_limit_array.append(min(x_array))
+                x_upper_limit_array.append(max(x_array))
+                y_array = get_data_array(data_dir_to_be_used, y_header_input)
+                y_lower_limit_array.append(min(y_array))
+                y_upper_limit_array.append(max(y_array))
+            except ValueError:
+                ignore_folder_array.append(folder)
 
         x_adjust_limit = {"lower_limit": int(min(x_lower_limit_array)),
                           "upper_limit": int(max(x_upper_limit_array))}
         y_adjust_limit = {"lower_limit": round(min(y_lower_limit_array), 2),
                           "upper_limit": round(max(y_upper_limit_array), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
+        if ignore_folder_array:
+            num_of_ignore_folder = len(ignore_folder_array)
+            if num_of_ignore_folder > 1:
+                print(f"{num_of_ignore_folder} folders are ignored because of value error.")
+            else:
+                print(f"{num_of_ignore_folder} folder is ignored because of value error.")
 
-    return x_adjust_limit, y_adjust_limit
+    return x_adjust_limit, y_adjust_limit, ignore_folder_array
 
 
 def get_draw_info_for_trial_plot(config_info_input, x_array_input, y_array_input):
     x_axis_limit = config_info_input["x_axis_limit"]
     y_axis_limit = config_info_input["y_axis_limit"]
     mean_offset = config_info_input["mean_offset"]
     axis_adjustment_types = config_info_input["axis_adjustment_types"]
@@ -1387,98 +1420,480 @@
                 # event_marker_time_f = float(event_marker_sts - start_marker)
                 # print(event_marker_time_f - event_marker_time_i)
                 event_marker_array.append(float(event_marker_sts - start_marker))
 
     return event_marker_array
 
 
-def get_config_location():
-    config_dir = pkg_resources.resource_filename("okntool", "oknserver_graph_plot_config.json")
-    return config_dir
+def get_config_location(config_name_input):
+    config_exist = config_resources.is_resource("okntool", config_name_input)
+    if config_exist:
+        with config_resources.path("okntool", config_name_input) as p:
+            config_location = p
+    else:
+        config_location = None
+    return config_location
+
+
+def draw_simpler_graph(folder_dir_input, config_input, referenced_csv_to_be_used):
+    graph_line_color = config_input["graph_line_color"]
+    graph_line_thickness = config_input["graph_line_thickness"]
+    x_label = config_input["x_label"]
+    x_label_x_position = config_input["x_label_x_position"]
+    x_label_y_position = config_input["x_label_y_position"]
+    x_label_alignment = config_input["x_label_alignment"]
+    x_label_rotation = config_input["x_label_rotation"]
+    x_label_weight = config_input["x_label_weight"]
+    x_label_font_size = config_input["x_label_font_size"]
+    y_label = config_input["y_label"]
+    y_label_x_position = config_input["y_label_x_position"]
+    y_label_y_position = config_input["y_label_y_position"]
+    y_label_alignment = config_input["y_label_alignment"]
+    y_label_rotation = config_input["y_label_rotation"]
+    y_label_weight = config_input["y_label_weight"]
+    y_label_font_size = config_input["y_label_font_size"]
+    main_boundary_position = config_input["main_boundary_position"]
+    main_boundary_width = config_input["main_boundary_width"]
+    main_boundary_height = config_input["main_boundary_height"]
+    main_boundary_color = config_input["main_boundary_color"]
+    main_boundary_line_thickness = config_input["main_boundary_line_thickness"]
+    image_scale = config_input["image_scale"]
+    axis_y_label_rotation = config_input["axis_y_label_rotation"]
+    axis_y_label_weight = config_input["axis_y_label_weight"]
+    axis_y_label_font_size = config_input["axis_y_label_font_size"]
+    axis_y_label_pad = config_input["axis_y_label_pad"]
+    mid_line = config_input["mid_line"]
+    mid_line_level = config_input["mid_line_level"]
+    mid_line_color = config_input["mid_line_color"]
+    mid_line_style = config_input["mid_line_style"]
+    mid_line_thickness = config_input["mid_line_thickness"]
+    axis_right_top_left_bottom_borders = config_input["axis_right_top_left_bottom_borders"]
+    subplots_space_adjustment = config_input["subplots_space_adjustment"]
+    subplots_width_space = config_input["subplots_width_space"]
+    subplots_height_space = config_input["subplots_height_space"]
+    time_notation = config_input["time_notation"]
+    time_notation_text_position = config_input["time_notation_text_position"]
+    time_notation_text_weight = config_input["time_notation_text_weight"]
+    time_notation_text_font_size = config_input["time_notation_text_font_size"]
+    time_line_x_position_start_end = config_input["time_line_x_position_start_end"]
+    time_line_y_position_start_end = config_input["time_line_y_position_start_end"]
+    time_line_style = config_input["time_line_style"]
+    time_line_color = config_input["time_line_color"]
+    time_line_thickness = config_input["time_line_thickness"]
+    time_boundary_position = config_input["time_boundary_position"]
+    time_boundary_width = config_input["time_boundary_width"]
+    time_boundary_height = config_input["time_boundary_height"]
+    time_boundary_color = config_input["time_boundary_color"]
+    time_boundary_line_thickness = config_input["time_boundary_line_thickness"]
+
+    plot_info, adjust_limit_info = get_plot_info_for_simpler(folder_dir_input, config_input, referenced_csv_to_be_used)
+
+    x_adjust_limit = adjust_limit_info["x_adjust_limit"]
+    x_lower_limit = x_adjust_limit["lower_limit"]
+    x_upper_limit = x_adjust_limit["upper_limit"]
+    y_adjust_limit = adjust_limit_info["y_adjust_limit"]
+    y_lower_limit = y_adjust_limit["lower_limit"]
+    y_upper_limit = y_adjust_limit["upper_limit"]
+
+    output_image_name = config_input["output_image_name"]
+    display_output_dir = os.path.join(folder_dir_input, output_image_name)
+
+    final_plot_array = []
+    for logmar_level in logmar_level_array:
+        temp_logmar_info_array = []
+
+        for info in plot_info:
+            if info["logmar"] == logmar_level:
+                temp_logmar_info_array.append(info)
+
+        if len(temp_logmar_info_array) > 0:
+            temp_dict = {"logmar_level": logmar_level, "info_array": temp_logmar_info_array}
+            final_plot_array.append(temp_dict)
+
+    if len(final_plot_array) > 0:
+        final_row_length = len(final_plot_array)
+        final_column_length = 0
+        for plot_info in final_plot_array:
+            info_array = plot_info["info_array"]
+            if len(info_array) > final_column_length:
+                final_column_length = len(info_array)
+
+        if final_row_length > 1:
+            plot_info_len = len(final_plot_array)
+            if plot_info_len <= 1:
+                print("There is only 1 logmar level in the given data.")
+                print("Therefore, we cannot draw tidy graph. It needs at least 2 logmar level.")
+            else:
+                fig, axs = plt.subplots(final_row_length, final_column_length,
+                                        figsize=(final_column_length * image_scale * 1,
+                                                 final_row_length * image_scale * 1))
+
+                for row_index, plot_info in enumerate(final_plot_array):
+                    logmar_level = plot_info["logmar_level"]
+                    info_array = plot_info["info_array"]
+                    info_array_length = len(info_array)
+                    num_plot_to_be_deleted = 0
+                    if info_array_length < int(final_column_length):
+                        num_plot_to_be_deleted = final_column_length - info_array_length
+                    for column_index, info in enumerate(info_array):
+                        x_array = info["x_array"]
+                        y_array = info["y_array"]
+                        sp_array = info["sp_array"]
+                        sp_line_color = info["sp_line_color"]
+                        sp_line_thickness = info["sp_line_thickness"]
+                        qp_array = info["qp_array"]
+                        qp_line_color = info["qp_line_color"]
+                        qp_line_thickness = info["qp_line_thickness"]
+                        axs[row_index, column_index].plot(x_array, y_array, color=graph_line_color,
+                                                          linewidth=graph_line_thickness)
+                        axs[row_index, column_index].plot(x_array, sp_array, color=sp_line_color,
+                                                          linewidth=sp_line_thickness)
+                        axs[row_index, column_index].plot(x_array, qp_array, color=qp_line_color,
+                                                          linewidth=qp_line_thickness)
+                        axs[row_index, column_index].set_xlim([x_lower_limit, x_upper_limit])
+                        axs[row_index, column_index].set_ylim([y_lower_limit, y_upper_limit])
+                        if type(logmar_level) is int or type(logmar_level) is float:
+                            axs[row_index, column_index].set_ylabel(str(logmar_level),
+                                                                    rotation=axis_y_label_rotation,
+                                                                    weight=axis_y_label_weight,
+                                                                    fontsize=axis_y_label_font_size,
+                                                                    labelpad=axis_y_label_pad)
+                        else:
+                            axs[row_index, column_index].set_ylabel(str("None  "),
+                                                                    rotation=axis_y_label_rotation,
+                                                                    weight=axis_y_label_weight,
+                                                                    fontsize=axis_y_label_font_size,
+                                                                    labelpad=axis_y_label_pad)
+                        axs[row_index, column_index].set_xticks([])
+                        axs[row_index, column_index].set_yticks([])
+                        if mid_line:
+                            axs[row_index, column_index].axhline(y=mid_line_level, color=mid_line_color,
+                                                                 linestyle=mid_line_style,
+                                                                 linewidth=mid_line_thickness)
+
+                        # Hide/Show the borders/spines
+                        for axx in axs.flat:
+                            axx.spines['right'].set_visible(axis_right_top_left_bottom_borders[0])
+                            axx.spines['top'].set_visible(axis_right_top_left_bottom_borders[1])
+                            axx.spines['left'].set_visible(axis_right_top_left_bottom_borders[2])
+                            axx.spines['bottom'].set_visible(axis_right_top_left_bottom_borders[3])
+
+                    if num_plot_to_be_deleted > 0:
+                        for index in range(num_plot_to_be_deleted):
+                            column_index_to_be_deleted = int(final_column_length) - (index + 1)
+                            axs[row_index, column_index_to_be_deleted].set_axis_off()
+
+                    # Hide all x axis labels inside the combined graph and show left and outside.
+                    for ax in axs.flat:
+                        ax.label_outer()
+
+                plt.tick_params(
+                    axis='x',  # changes apply to the x-axis
+                    which='both',
+                    left=False,
+                    right=False,  # both major and minor ticks are affected
+                    bottom=False,  # ticks along the bottom edge are off
+                    top=False,  # ticks along the top edge are off
+                    labelbottom=False)  # labels along the bottom edge are off
+                plt.tick_params(
+                    axis='y',  # changes apply to the y-axis
+                    which='both',
+                    left=False,
+                    right=False,  # both major and minor ticks are affected
+                    bottom=False,  # ticks along the bottom edge are off
+                    top=False,  # ticks along the top edge are off
+                    labelbottom=False)  # labels along the bottom edge are off
+                plt.xticks([]), plt.yticks([])
+
+                if subplots_space_adjustment:
+                    plt.subplots_adjust(wspace=subplots_width_space, hspace=subplots_height_space)
+
+                fig.text(x_label_x_position, x_label_y_position, x_label,
+                         ha=x_label_alignment, rotation=x_label_rotation,
+                         weight=x_label_weight, fontsize=x_label_font_size)
+                fig.text(y_label_x_position, y_label_y_position, y_label,
+                         va=y_label_alignment, rotation=y_label_rotation,
+                         weight=y_label_weight, fontsize=y_label_font_size)
+                main_boundary = plt.Rectangle(
+                    # (x,y at lower-left corner), width, height
+                    (main_boundary_position[0], main_boundary_position[1]),
+                    main_boundary_width, main_boundary_height,
+                    fill=False, color=main_boundary_color,
+                    lw=main_boundary_line_thickness,
+                    zorder=1000, transform=fig.transFigure,
+                    figure=fig
+                )
+                if time_notation and time_notation != "none":
+                    fig.text(time_notation_text_position[0],
+                             time_notation_text_position[1],
+                             time_notation,
+                             weight=time_notation_text_weight,
+                             fontsize=time_notation_text_font_size)
+                    fig.add_artist(Line2D(time_line_x_position_start_end, time_line_y_position_start_end,
+                                          linestyle=time_line_style, color=time_line_color,
+                                          linewidth=time_line_thickness))
+                    time_notation_boundary = plt.Rectangle(
+                        # (x,y at lower-left corner), width, height
+                        (time_boundary_position[0], time_boundary_position[1]),
+                        time_boundary_width, time_boundary_height,
+                        fill=False, color=time_boundary_color,
+                        lw=time_boundary_line_thickness,
+                        zorder=1000, transform=fig.transFigure,
+                        figure=fig
+                    )
+                    fig.patches.extend([main_boundary, time_notation_boundary])
+                else:
+                    fig.patches.extend([main_boundary])
+                os.chdir(folder_dir_input)
+                fig.savefig(output_image_name)
+                plt.close()
+            print(f"Tidy plot has been saved at:{display_output_dir}")
+        else:
+            print("There is only 1 logmar level in the given data.")
+            print("Therefore, we cannot draw tidy graph. It needs at least 2 logmar level.")
+    else:
+        print("There is nothing to plot")
+
+
+def get_plot_info_for_simpler(data_dir, plot_info_input, referenced_csv_dir_input):
+    x_label = plot_info_input["x_label"]
+    y_label = plot_info_input["y_label"]
+    x_data_column_name = plot_info_input["x_data_column_name"]
+    y_data_column_name = plot_info_input["y_data_column_name"]
+    x_axis_limit = plot_info_input["x_axis_limit"]
+    y_axis_limit = plot_info_input["y_axis_limit"]
+    mean_offset = plot_info_input["mean_offset"]
+    axis_adjustment_types = plot_info_input["axis_adjustment_types"]
+    axis_adjustment_type_number = plot_info_input["axis_adjustment_type_number"]
+    signal_csv_folder_name = plot_info_input["signal_csv_folder_name"]
+    signal_csv_name = plot_info_input["signal_csv_name"]
+    sp_column_name = plot_info_input["sp_column_name"]
+    qp_column_name = plot_info_input["qp_column_name"]
+    sp_line_color = plot_info_input["sp_line_color"]
+    sp_line_thickness = plot_info_input["sp_line_thickness"]
+    qp_line_color = plot_info_input["qp_line_color"]
+    qp_line_thickness = plot_info_input["qp_line_thickness"]
+    info_array = get_info_array_for_simpler_plot(referenced_csv_dir_input, "logMAR", "filename")
+    folder_array = [info[2] for info in info_array]
+    # print(folder_array)
+
+    adjustment_type = axis_adjustment_types[str(axis_adjustment_type_number)]
+    if adjustment_type == "mean_offset":
+        plot_info_array = []
+        x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, signal_csv_name,
+                                                                               x_data_column_name, y_data_column_name,
+                                                                               folder_array, x_axis_limit,
+                                                                               y_axis_limit, mean_offset,
+                                                                               axis_adjustment_types,
+                                                                               axis_adjustment_type_number)
+        adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        if ignore_folder_array:
+            info_array = [info for info in info_array if info[2] not in ignore_folder_array]
+        for trial_id, logmar_level, folder_name in info_array:
+            signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_name)
+            x_array = get_data_array(signal_csv_dir, x_data_column_name)
+            y_array = get_data_array(signal_csv_dir, y_data_column_name)
+            y_mean = np.nanmean(y_array)
+            y_array = [value - y_mean for value in y_array]
+            sp_array, qp_array = get_sp_and_qp_array(signal_csv_dir, sp_column_name, qp_column_name,
+                                                     y_array)
+            plot_info = {"trial_id": trial_id, "disk_condition": str(logmar_level),
+                         "x_label": x_label, "y_label": y_label,
+                         "x_array": x_array, "y_array": y_array,
+                         "sp_array": sp_array, "qp_array": qp_array,
+                         "sp_line_color": sp_line_color, "sp_line_thickness": sp_line_thickness,
+                         "qp_line_color": qp_line_color, "qp_line_thickness": qp_line_thickness,
+                         "logmar": disk_to_logmar(logmar_level)}
+            plot_info_array.append(plot_info)
+    else:
+        plot_info_array = []
+        x_adjust_limit, y_adjust_limit, ignore_folder_array = get_adjust_limit(data_dir, signal_csv_name,
+                                                                               x_data_column_name, y_data_column_name,
+                                                                               folder_array, x_axis_limit,
+                                                                               y_axis_limit, mean_offset,
+                                                                               axis_adjustment_types,
+                                                                               axis_adjustment_type_number)
+        adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
+        if ignore_folder_array:
+            info_array = [info for info in info_array if info[2] not in ignore_folder_array]
+        for trial_id, logmar_level, folder_name in info_array:
+            signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_name)
+            x_array = get_data_array(signal_csv_dir, x_data_column_name)
+            y_array = get_data_array(signal_csv_dir, y_data_column_name)
+            sp_array, qp_array = get_sp_and_qp_array(signal_csv_dir, sp_column_name, qp_column_name,
+                                                     y_array)
+            plot_info = {"trial_id": trial_id, "disk_condition": logmar_level,
+                         "x_label": x_label, "y_label": y_label,
+                         "x_array": x_array, "y_array": y_array,
+                         "sp_array": sp_array, "qp_array": qp_array,
+                         "sp_line_color": sp_line_color, "sp_line_thickness": sp_line_thickness,
+                         "qp_line_color": qp_line_color, "qp_line_thickness": qp_line_thickness,
+                         "logmar": disk_to_logmar(logmar_level)}
+            plot_info_array.append(plot_info)
+
+    return plot_info_array, adjust_limit_dict
+
+
+def get_info_array_for_simpler_plot(referenced_csv_dir, logmar_header_input, file_name_header_input):
+    file_to_open = open(referenced_csv_dir)
+    csv_reader = csv.reader(file_to_open)
+    header_array = []
+    rows = []
+    count_one = 0
+    output_array = []
+
+    for row in csv_reader:
+        if count_one <= 0:
+            header_array = row
+            count_one += 1
+        else:
+            rows.append(row)
+
+    file_name_header_position = get_index(file_name_header_input, header_array)
+    logmar_header_position = get_index(logmar_header_input, header_array)
+
+    for row in rows:
+        raw_file_name = str(row[file_name_header_position])
+        logmar_level = float(row[logmar_header_position])
+        folder_name = raw_file_name[raw_file_name.find("./") + 2:raw_file_name.find(".mp4")]
+        trial_id = folder_name[folder_name.find("trial-"):folder_name.find("-disks")]
+        output_array.append([trial_id, logmar_level, folder_name])
+
+    return output_array
 
 
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='3.0.0'),
+    parser.add_argument('--version', action='version', version='4.0.0'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
-                        help="trial, summary, (staircase or progress) or tidy", metavar="plot type")
+                        help="trial, summary, (staircase or progress), tidy or simpler", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
-                        help=f"config file to be used", metavar="config location")
+                        help="config file to be used", metavar="config location")
+    parser.add_argument("-r", dest="referenced_csv", required=False, default=sys.stdin,
+                        help="csv file to be referenced", metavar="referenced csv location")
 
     args = parser.parse_args()
     directory_input = str(args.directory_input)
     type_input = str(args.plot_type)
     config_file_location = str(args.config_dir)
-    config_location = None
+    referenced_csv_dir = str(args.referenced_csv)
+    config_dir_exist = False
+    config_input = False if "_io.TextIOWrapper" in config_file_location else True
+    referenced_csv_input = False if "_io.TextIOWrapper" in referenced_csv_dir else True
+    # config_name_dict = {}
+    # config_name_dict["trial"] = "oknserver_graph_plot_config.json"
+    # config_name_dict["summary"] = "oknserver_graph_plot_config.json"
+    # config_name_dict["staircase"] = "oknserver_graph_plot_config.json"
+    # config_name_dict["progress"] = "oknserver_graph_plot_config.json"
+    # config_name_dict["tidy"] = "oknserver_graph_plot_config.json"
+    # config_name_dict["simpler"] = "simpler_plot_config.json"
+    config_name_dict = {"trial": "oknserver_graph_plot_config.json", "summary": "oknserver_graph_plot_config.json",
+                        "staircase": "oknserver_graph_plot_config.json", "progress": "oknserver_graph_plot_config.json",
+                        "tidy": "oknserver_graph_plot_config.json", "simpler": "simpler_plot_config.json"}
+
+    config_name = config_name_dict[type_input]
 
     # print(config_file_location)
-    if "_io.TextIOWrapper" in config_file_location:
-        config_location = get_config_location()
-        print(f"Therefore, okntool is using build-in config: {config_location}.")
-        config_build_in_exist = os.path.isfile(config_location)
-        if not config_build_in_exist:
+    if not config_input:
+        print("There is no config input.")
+        config_location = get_config_location(config_name)
+        if config_location:
+            print(f"Therefore, okntool is using built-in config: {config_location}.")
+            config_dir_exist = True
+        else:
             print(f"Error in retrieving config:{config_location}.")
             return
     else:
         config_dir_exist = os.path.isfile(config_file_location)
         if not config_dir_exist:
             print(f"Config location input:{config_file_location} does not exist.")
+            return
         else:
             config_location = config_file_location
             print(f"Config location input:{directory_input} is valid.")
 
     print("------------------")
     print(f"OKN TOOL PLOT INFO")
     print(f"Input directory:{directory_input}")
     print(f"Plot type:{type_input}")
     print(f"Config: {config_location}")
 
     # check whether input directory exists or not
     dir_exist = os.path.isdir(directory_input)
     if not dir_exist:
-        f"Directory input:{directory_input} does not exist"
+        print(f"Directory input:{directory_input} does not exist.")
+        print(f"Therefore, okntool could not process {type_input}")
         return
     else:
-        f"Directory input:{directory_input} is valid"
+        print(f"Directory input:{directory_input} is valid.")
 
-    # Opening oknserver graph plot config
-    with open(config_location) as f:
-        plot_config_info = json.load(f)
+    if config_dir_exist and dir_exist:
+        try:
+            # Opening oknserver graph plot config
+            with open(config_location) as f:
+                plot_config_info = json.load(f)
+        except FileNotFoundError:
+            plot_config_info = None
         if plot_config_info is not None:
-            print("oknserver_graph_plot_config.json is found.")
+            print(f"{config_name} is found.")
         else:
-            print("Essential config file oknserver_graph_plot_config.json is missing.")
-
-        if plot_config_info is not None and dir_exist:
-            if type_input == "trial":
-                # Retrieve trial plot info from config
-                trial_plot_info = plot_config_info["trial_plot"]
-
-                csv_name = f"updated_{os.path.basename(directory_input)}.csv"
-                print(f"csv name {csv_name}")
-                updated_csv_dir = os.path.join(directory_input, csv_name)
-                print(f"update csv dir {updated_csv_dir}")
-                signal_csv_folder_name = trial_plot_info["signal_csv_folder_name"]
-                signal_csv_name = trial_plot_info["signal_csv_name"]
-                signal_csv_dir = os.path.join(directory_input, signal_csv_folder_name, signal_csv_name)
-                print(f"signal csv dir {signal_csv_dir}")
-                draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir)
-            elif type_input == "summary":
-                # Retrieve summary plot info from config
-                summary_plot_info = plot_config_info["summary_plot"]
-
-                plot_combined_graph(directory_input, summary_plot_info)
-            elif type_input == "staircase" or type_input == "progress":
-                # Retrieve progress plot info from config
-                progress_plot_info = plot_config_info["progress_plot"]
-
-                draw_progress_graph(directory_input, progress_plot_info)
-            elif type_input == "tidy":
-                # Retrieve progress plot info from config
-                tidy_plot_info = plot_config_info["tidy_plot"]
+            print(f"Essential config file:{config_name} is missing.")
+    else:
+        plot_config_info = None
 
-                draw_tidy_graph(directory_input, tidy_plot_info)
+    if config_dir_exist and dir_exist and plot_config_info is not None:
+        if type_input == "trial":
+            # Retrieve trial plot info from config
+            trial_plot_info = plot_config_info["trial_plot"]
+
+            csv_name = f"updated_{os.path.basename(directory_input)}.csv"
+            print(f"csv name {csv_name}")
+            updated_csv_dir = os.path.join(directory_input, csv_name)
+            print(f"update csv dir {updated_csv_dir}")
+            signal_csv_folder_name = trial_plot_info["signal_csv_folder_name"]
+            signal_csv_name = trial_plot_info["signal_csv_name"]
+            signal_csv_dir = os.path.join(directory_input, signal_csv_folder_name, signal_csv_name)
+            print(f"signal csv dir {signal_csv_dir}")
+            draw_graph_with_overlay(updated_csv_dir, trial_plot_info, signal_csv_dir)
+        elif type_input == "summary":
+            # Retrieve summary plot info from config
+            summary_plot_info = plot_config_info["summary_plot"]
+
+            plot_combined_graph(directory_input, summary_plot_info)
+        elif type_input == "staircase" or type_input == "progress":
+            # Retrieve progress plot info from config
+            progress_plot_info = plot_config_info["progress_plot"]
+
+            draw_progress_graph(directory_input, progress_plot_info)
+        elif type_input == "tidy":
+            # Retrieve progress plot info from config
+            tidy_plot_info = plot_config_info["tidy_plot"]
+
+            draw_tidy_graph(directory_input, tidy_plot_info)
+        elif type_input == "simpler":
+            # Retrieve progress plot info from config
+            simpler_plot_info = plot_config_info["simpler_plot"]
+            if referenced_csv_input:
+                draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
             else:
-                print("wrong plot type or invalid plot type.")
+                print("There is no referenced csv input in the commandline.")
+                try:
+                    referenced_csv_name = simpler_plot_info["summary_csv_name"]
+                except KeyError:
+                    print("There is no referenced csv info in the config.")
+                    referenced_csv_name = "protocol.simpler.csv"
+                    print(f"Therefore using default name => {referenced_csv_name} as default referenced csv")
+                one_folder_back_dir = os.path.abspath(os.path.join(directory_input, os.pardir))
+                two_folder_back_dir = os.path.abspath(os.path.join(one_folder_back_dir, os.pardir))
+                referenced_csv_dir = os.path.join(two_folder_back_dir, referenced_csv_name)
+                referenced_csv_dir_exist = os.path.isfile(referenced_csv_dir)
+                if referenced_csv_dir_exist:
+                    draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
+                else:
+                    print(f"{referenced_csv_name} could not find in the directory:{two_folder_back_dir}")
+        else:
+            print("wrong plot type or invalid plot type.")
+    else:
+        return
```

### Comparing `okntool-3.0.0/okntool.egg-info/PKG-INFO` & `okntool-4.0.0/okntool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 3.0.0
+Version: 4.0.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-3.0.0/setup.py` & `okntool-4.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='3.0.0',
+    version='4.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
     packages=find_packages(),
     include_package_data=True,
-    package_data={'': ['oknserver_graph_plot_config.json']},
+    package_data={'': ['oknserver_graph_plot_config.json', 'simpler_plot_config.json']},
     entry_points={
         'console_scripts': [
             'okntool = okntool.okntool:main'
         ]
     },
     classifiers=[
         "Programming Language :: Python :: 3",
```

