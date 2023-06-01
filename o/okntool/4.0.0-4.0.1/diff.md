# Comparing `tmp/okntool-4.0.0.tar.gz` & `tmp/okntool-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-4.0.0.tar", last modified: Thu Jun  1 08:24:33 2023, max compression
+gzip compressed data, was "okntool-4.0.1.tar", last modified: Thu Jun  1 08:32:47 2023, max compression
```

## Comparing `okntool-4.0.0.tar` & `okntool-4.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.189015 okntool-4.0.0/
--rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.0/LICENSE
--rw-rw-rw-   0        0        0      555 2023-06-01 08:24:33.187587 okntool-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.180604 okntool-4.0.0/okntool/
--rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.0/okntool/__init__.py
--rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.0/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0   102106 2023-06-01 08:13:39.000000 okntool-4.0.0/okntool/okntool.py
--rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.0/okntool/simpler_plot_config.json
-drwxrwxrwx   0        0        0        0 2023-06-01 08:24:33.187587 okntool-4.0.0/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-01 08:24:17.000000 okntool-4.0.0/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 08:24:33.000000 okntool-4.0.0/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:24:33.189015 okntool-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-05-31 03:13:16.000000 okntool-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.559367 okntool-4.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-4.0.1/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:32:47.558367 okntool-4.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-4.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.550196 okntool-4.0.1/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-4.0.1/okntool/__init__.py
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-4.0.1/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0   102255 2023-06-01 08:31:58.000000 okntool-4.0.1/okntool/okntool.py
+-rw-rw-rw-   0        0        0     2426 2023-06-01 08:22:38.000000 okntool-4.0.1/okntool/simpler_plot_config.json
+drwxrwxrwx   0        0        0        0 2023-06-01 08:32:47.558367 okntool-4.0.1/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-01 08:32:42.000000 okntool-4.0.1/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 08:32:47.000000 okntool-4.0.1/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 08:32:47.559367 okntool-4.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-06-01 08:31:58.000000 okntool-4.0.1/setup.py
```

### Comparing `okntool-4.0.0/LICENSE` & `okntool-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-4.0.0/PKG-INFO` & `okntool-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.0
+Version: 4.0.1
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.0/README.md` & `okntool-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `okntool-4.0.0/okntool/oknserver_graph_plot_config.json` & `okntool-4.0.1/okntool/oknserver_graph_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.0/okntool/okntool.py` & `okntool-4.0.1/okntool/okntool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1760,15 +1760,15 @@
 
     return output_array
 
 
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='4.0.0'),
+    parser.add_argument('--version', action='version', version='4.0.1'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
                         help="trial, summary, (staircase or progress), tidy or simpler", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
                         help="config file to be used", metavar="config location")
     parser.add_argument("-r", dest="referenced_csv", required=False, default=sys.stdin,
@@ -1886,14 +1886,16 @@
                     referenced_csv_name = "protocol.simpler.csv"
                     print(f"Therefore using default name => {referenced_csv_name} as default referenced csv")
                 one_folder_back_dir = os.path.abspath(os.path.join(directory_input, os.pardir))
                 two_folder_back_dir = os.path.abspath(os.path.join(one_folder_back_dir, os.pardir))
                 referenced_csv_dir = os.path.join(two_folder_back_dir, referenced_csv_name)
                 referenced_csv_dir_exist = os.path.isfile(referenced_csv_dir)
                 if referenced_csv_dir_exist:
+                    print(f"Default referenced csv location:{referenced_csv_dir} is found.")
+                    print("Start plotting simpler plot...")
                     draw_simpler_graph(directory_input, simpler_plot_info, referenced_csv_dir)
                 else:
-                    print(f"{referenced_csv_name} could not find in the directory:{two_folder_back_dir}")
+                    print(f"Default referenced csv location:{referenced_csv_dir} cannot be found.")
         else:
             print("wrong plot type or invalid plot type.")
     else:
         return
```

### Comparing `okntool-4.0.0/okntool/simpler_plot_config.json` & `okntool-4.0.1/okntool/simpler_plot_config.json`

 * *Files identical despite different names*

### Comparing `okntool-4.0.0/okntool.egg-info/PKG-INFO` & `okntool-4.0.1/okntool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 4.0.0
+Version: 4.0.1
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-4.0.0/setup.py` & `okntool-4.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='4.0.0',
+    version='4.0.1',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

