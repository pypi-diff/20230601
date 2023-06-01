# Comparing `tmp/okntool-4.0.1.tar.gz` & `tmp/okntool-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-4.0.1.tar", last modified: Thu Jun  1 08:32:47 2023, max compression
+gzip compressed data, was "okntool-4.0.2.tar", last modified: Thu Jun  1 08:36:23 2023, max compression
```

## Comparing `okntool-4.0.1.tar` & `okntool-4.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.559367 okntool-4.0.1/
--rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.1/LICENSE
--rw-rw-rw-   0        0        0      555 2023-06-01 08:32:47.558367 okntool-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.550196 okntool-4.0.1/okntool/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.1/okntool/__init__.py
--rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.1/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0   102255 2023-06-01 08:31:58.000000 okntool-4.0.1/okntool/okntool.py
--rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.1/okntool/simpler_plot_config.json
-drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.558367 okntool-4.0.1/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 08:32:42.000000 okntool-4.0.1/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:32:47.559367 okntool-4.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-06-01 08:31:58.000000 okntool-4.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.497352 okntool-4.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.2/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:36:23.497352 okntool-4.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.489372 okntool-4.0.2/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.2/okntool/__init__.py
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.2/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0   102264 2023-06-01 08:35:44.000000 okntool-4.0.2/okntool/okntool.py
+-rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.2/okntool/simpler_plot_config.json
+drwxrwxrwx   0        0        0        0 2023-06-01 08:36:23.496356 okntool-4.0.2/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 08:36:13.000000 okntool-4.0.2/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 08:36:23.000000 okntool-4.0.2/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:36:23.497352 okntool-4.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-06-01 08:35:44.000000 okntool-4.0.2/setup.py
```

### Comparing `okntool-4.0.1/LICENSE` & `okntool-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-4.0.1/PKG-INFO` & `okntool-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.1
+Version: 4.0.2
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.1/README.md` & `okntool-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `okntool-4.0.1/okntool/oknserver_graph_plot_config.json` & `okntool-4.0.2/okntool/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.1/okntool/okntool.py` & `okntool-4.0.2/okntool/okntool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1517,15 +1517,15 @@
             if len(info_array) > final_column_length:
                 final_column_length = len(info_array)
 
         if final_row_length > 1:
             plot_info_len = len(final_plot_array)
             if plot_info_len <= 1:
                 print("There is only 1 logmar level in the given data.")
-                print("Therefore, we cannot draw tidy graph. It needs at least 2 logmar level.")
+                print("Therefore, we cannot draw simpler graph. It needs at least 2 logmar level.")
             else:
                 fig, axs = plt.subplots(final_row_length, final_column_length,
                                         figsize=(final_column_length * image_scale * 1,
                                                  final_row_length * image_scale * 1))
 
                 for row_index, plot_info in enumerate(final_plot_array):
                     logmar_level = plot_info["logmar_level"]
@@ -1642,18 +1642,18 @@
                     )
                     fig.patches.extend([main_boundary, time_notation_boundary])
                 else:
                     fig.patches.extend([main_boundary])
                 os.chdir(folder_dir_input)
                 fig.savefig(output_image_name)
                 plt.close()
-            print(f"Tidy plot has been saved at:{display_output_dir}")
+            print(f"Simpler plot has been saved at:{display_output_dir}")
         else:
             print("There is only 1 logmar level in the given data.")
-            print("Therefore, we cannot draw tidy graph. It needs at least 2 logmar level.")
+            print("Therefore, we cannot draw simpler graph. It needs at least 2 logmar level.")
     else:
         print("There is nothing to plot")
 
 
 def get_plot_info_for_simpler(data_dir, plot_info_input, referenced_csv_dir_input):
     x_label = plot_info_input["x_label"]
     y_label = plot_info_input["y_label"]
@@ -1760,15 +1760,15 @@
 
     return output_array
 
 
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='4.0.1'),
+    parser.add_argument('--version', action='version', version='4.0.2'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
                         help="trial, summary, (staircase or progress), tidy or simpler", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
                         help="config file to be used", metavar="config location")
     parser.add_argument("-r", dest="referenced_csv", required=False, default=sys.stdin,
```

### Comparing `okntool-4.0.1/okntool/simpler_plot_config.json` & `okntool-4.0.2/okntool/simpler_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.1/okntool.egg-info/PKG-INFO` & `okntool-4.0.2/okntool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.1
+Version: 4.0.2
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.1/setup.py` & `okntool-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='4.0.1',
+    version='4.0.2',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

