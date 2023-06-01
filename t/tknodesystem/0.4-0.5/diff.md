# Comparing `tmp/tknodesystem-0.4.tar.gz` & `tmp/tknodesystem-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tknodesystem-0.4.tar", last modified: Sun May 21 13:36:59 2023, max compression
+gzip compressed data, was "tknodesystem-0.5.tar", last modified: Thu Jun  1 09:08:33 2023, max compression
```

## Comparing `tknodesystem-0.4.tar` & `tknodesystem-0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.105709 tknodesystem-0.4/
--rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.4/LICENSE
--rw-rw-rw-   0        0        0     2621 2023-05-21 13:36:59.105709 tknodesystem-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-05-20 06:28:49.000000 tknodesystem-0.4/README.md
--rw-rw-rw-   0        0        0      570 2023-05-21 13:36:59.105709 tknodesystem-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-21 13:36:37.000000 tknodesystem-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.027585 tknodesystem-0.4/tknodesystem/
--rw-rw-rw-   0        0        0      278 2023-05-21 12:58:35.000000 tknodesystem-0.4/tknodesystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.090084 tknodesystem-0.4/tknodesystem/grid_images/
--rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.4/tknodesystem/grid_images/grid_dot.png
--rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.4/tknodesystem/grid_images/grid_lines.png
--rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.4/tknodesystem/grid_images/no_grid.png
--rw-rw-rw-   0        0        0     4693 2023-05-20 06:06:47.000000 tknodesystem-0.4/tknodesystem/node.py
--rw-rw-rw-   0        0        0     3096 2023-05-21 13:28:36.000000 tknodesystem-0.4/tknodesystem/node_args.py
--rw-rw-rw-   0        0        0    11797 2023-05-19 11:52:04.000000 tknodesystem-0.4/tknodesystem/node_canvas.py
--rw-rw-rw-   0        0        0     9357 2023-05-21 13:31:59.000000 tknodesystem-0.4/tknodesystem/node_menu.py
--rw-rw-rw-   0        0        0     4549 2023-05-17 06:00:55.000000 tknodesystem-0.4/tknodesystem/node_socket.py
--rw-rw-rw-   0        0        0    31644 2023-05-21 13:28:12.000000 tknodesystem-0.4/tknodesystem/node_types.py
--rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.4/tknodesystem/node_wire.py
-drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.058835 tknodesystem-0.4/tknodesystem.egg-info/
--rw-rw-rw-   0        0        0     2621 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.399585 tknodesystem-0.5/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.5/LICENSE
+-rw-rw-rw-   0        0        0     2711 2023-06-01 09:08:33.399585 tknodesystem-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2142 2023-06-01 08:59:10.000000 tknodesystem-0.5/README.md
+-rw-rw-rw-   0        0        0      570 2023-06-01 09:08:33.402587 tknodesystem-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-06-01 08:55:45.000000 tknodesystem-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.367100 tknodesystem-0.5/tknodesystem/
+-rw-rw-rw-   0        0        0      278 2023-05-23 07:46:35.000000 tknodesystem-0.5/tknodesystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.387365 tknodesystem-0.5/tknodesystem/grid_images/
+-rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.5/tknodesystem/grid_images/grid_dot.png
+-rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.5/tknodesystem/grid_images/grid_lines.png
+-rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.5/tknodesystem/grid_images/no_grid.png
+-rw-rw-rw-   0        0        0     4747 2023-06-01 06:29:09.000000 tknodesystem-0.5/tknodesystem/node.py
+-rw-rw-rw-   0        0        0     3175 2023-06-01 09:02:46.000000 tknodesystem-0.5/tknodesystem/node_args.py
+-rw-rw-rw-   0        0        0    11797 2023-06-01 07:12:09.000000 tknodesystem-0.5/tknodesystem/node_canvas.py
+-rw-rw-rw-   0        0        0     9395 2023-05-23 07:46:16.000000 tknodesystem-0.5/tknodesystem/node_menu.py
+-rw-rw-rw-   0        0        0     5147 2023-06-01 06:43:40.000000 tknodesystem-0.5/tknodesystem/node_socket.py
+-rw-rw-rw-   0        0        0    33308 2023-06-01 08:14:13.000000 tknodesystem-0.5/tknodesystem/node_types.py
+-rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.5/tknodesystem/node_wire.py
+drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.387365 tknodesystem-0.5/tknodesystem.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/top_level.txt
```

### Comparing `tknodesystem-0.4/LICENSE` & `tknodesystem-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/PKG-INFO` & `tknodesystem-0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.4
+Version: 0.5
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
-Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
+Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes,visual-scripting
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,15 +19,15 @@
 
 ## Feature
 - Lightweight library
 - Easy to install and use
 - Multiple nodes and inputs
 - **Save/Load** node trees
 - Canvas with **drag and zoom** ability
-- Customizable options
+- Customizable nodes and options
 - Built-in **Node menu**
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
@@ -56,14 +56,14 @@
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
 [<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
-Examples are given in the `examples` folder
+Examples are given in the [`examples`](https://github.com/Akascape/TkNodeSystem/tree/main/examples) folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
 **So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.4/README.md` & `tknodesystem-0.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Feature
 - Lightweight library
 - Easy to install and use
 - Multiple nodes and inputs
 - **Save/Load** node trees
 - Canvas with **drag and zoom** ability
-- Customizable options
+- Customizable nodes and options
 - Built-in **Node menu**
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
@@ -41,14 +41,14 @@
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
 [<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
-Examples are given in the `examples` folder
+Examples are given in the [`examples`](https://github.com/Akascape/TkNodeSystem/tree/main/examples) folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
 **So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.4/setup.cfg` & `tknodesystem-0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b6e 6f64 6573 7973 7465 6d0d   = tknodesystem.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 0d0a  .version = 0.4..
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 0d0a  .version = 0.5..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5369  description = Si
 00000040: 6d70 6c65 2056 6973 7561 6c20 4e6f 6465  mple Visual Node
 00000050: 2073 7973 7465 6d20 7769 7468 2054 6b69   system with Tki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `tknodesystem-0.4/setup.py` & `tknodesystem-0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tknodesystem',
-    version = '0.4',
+    version = '0.5',
     description = "Simple visual node system (DAG) with tkinter!",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/TkNodeSystem",
@@ -20,13 +20,13 @@
     classifiers = [
         "License :: OSI Approved :: MIT License ",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     keywords = ['customtkinter', 'tkinter', 'tkinter-nodes',
                 'tknodes', 'tkinter-DAG', 'node-system',
-                'node-based-ui', 'tknodesystem', 'nodes'],
+                'node-based-ui', 'tknodesystem', 'nodes', 'visual-scripting'],
     packages = ["tknodesystem", "tknodesystem.grid_images"],
     install_requires = ['customtkinter'],
     dependency_links = ['https://pypi.org/project/customtkinter/'],
     python_requires = '>=3.6',
 )
```

### Comparing `tknodesystem-0.4/tknodesystem/grid_images/grid_dot.png` & `tknodesystem-0.5/tknodesystem/grid_images/grid_dot.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/tknodesystem/grid_images/grid_lines.png` & `tknodesystem-0.5/tknodesystem/grid_images/grid_lines.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/tknodesystem/grid_images/no_grid.png` & `tknodesystem-0.5/tknodesystem/grid_images/no_grid.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/tknodesystem/node.py` & `tknodesystem-0.5/tknodesystem/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 class Node:
-    def __init__(self, canvas, width=50, height=50, border_color='white', border_width=0,
+    def __init__(self, canvas, width=50, height=50, border_color='white', border_width=0, justify="center",
                  fg_color='#37373D', center=(100,50), text='', text_color='white', corner_radius=25,
                  font=("",10), click_command=None, highlightcolor='#52d66c', hover=True):
         
         self.canvas = canvas
         self.width = width 
         self.height = height 
         self.node_outline_color = border_color
         self.node_outline_thickness = border_width
         self.node_color = fg_color
         self.text_color = text_color
         self.corner_radius = corner_radius
         self.font = font
+        self.justify = justify
         self.text = text
         self.center = center
         self.click_command = click_command
         self.auxlist = []
         self.signal = False
         self.hover = hover
         self.hover_color = highlightcolor
@@ -26,15 +27,15 @@
         """ create round rectangular frame with text """
         
         self.ID = self.create_round_rectangle(self.center[0]-self.width*0.5, self.center[1]-self.height*0.5,
                                               self.center[0]+self.width*0.5, self.center[1]+self.height*0.5,
                                               radius=self.corner_radius, outline=self.node_outline_color, fill=self.node_color,
                                               width=self.node_outline_thickness)
         
-        self.IDtext = self.canvas.create_text(self.center, fill=self.text_color, justify="center", font=self.font, text=self.text)
+        self.IDtext = self.canvas.create_text(self.center, fill=self.text_color, justify=self.justify, font=self.font, text=self.text)
         self.allIDs = [self.ID, self.IDtext]
         self.auxlist = [self.ID, self.IDtext]
 
         for i in self.auxlist:
             self.canvas.tag_bind(i, "<Button-1>", self.getpos, add="+")
             self.canvas.tag_bind(i, '<Enter>', self.enter_node)
             self.canvas.tag_bind(i, '<Leave>', self.leave_node)
```

### Comparing `tknodesystem-0.4/tknodesystem/node_args.py` & `tknodesystem-0.5/tknodesystem/node_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,60 @@
 class Args():
     """ This class is used to remove default arguments in order to reduce the size of the export file """
     
     def value_args(args):        
-        default_args ={'width': 100, 'height': 50, 'value': 0, 'border_color': 'white', 'text': None,
+        default_args = {'width': 100, 'height': 50, 'value': 0, 'border_color': 'white', 'text': None, 
                         'corner_radius': 25, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white',
                         'font': ('', 10), 'socket_radius': 8, 'socket_hover': True, 'socket_color': 'green',
-                        'socket_hover_color': 'grey50', 'highlightcolor': '#52d66c', 'hover': True,
-                        'click_command': None, 'side': 'right', 'x': None, 'y': None, 'num': None}
+                        'socket_hover_color': 'grey50', 'highlightcolor': '#52d66c', 'hover': True, 
+                        'click_command': None, 'side': 'right', 'x': None, 'y': None, 'num': None, 'justify': 'center'}
 
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("x")
         args.pop("y")
         args.pop("click_command")
         args.pop("num")
-
         new_args = {}
         
         for i in args.keys():
             if default_args.get(i)!=args.get(i):
                 new_args.update({i:args.get(i)})
 
         return new_args
     
     def func_args(args):
         default_args = {'width': 100, 'height': 80, 'inputs': 2, 'border_color': '#37373D', 'text': None, 'socket_radius': 8,
                         'corner_radius': 25, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white', 'font': ('', 10),
                         'highlightcolor': '#52d66c', 'hover': True, 'socket_color': 'green', 'socket_hover_color': 'grey50',
                         'x': None, 'y': None, 'multiside': False, 'output_socket_color': 'green', 'click_command': None,
-                        'socket_hover': True, 'num': None, 'none_inputs': False}
+                        'socket_hover': True, 'num': None, 'none_inputs': False, 'justify': 'center', 'hover_text': None}
 
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("command")
         args.pop("x")
         args.pop("y")
         args.pop("click_command")
         args.pop("num")
-
         new_args = {}
         
         for i in args.keys():
             if default_args.get(i)!=args.get(i):
                 new_args.update({i:args.get(i)})
 
         return new_args
 
     def compile_args(args):
-        default_args = {'width': 100, 'height': 50, 'border_color': '#37373D', 'text': 'Compile', 'socket_radius': 8,
-                         'corner_radius': 25, 'x': None, 'y': None, 'border_width': 0, 'fg_color': '#37373D', 'text_color':
-                         'white', 'font': ('', 10), 'highlightcolor': '#52d66c', 'hover': True, 'socket_hover': True, 'socket_color': 'green',
-                         'socket_hover_color': 'grey50', 'show_value': True, 'command': None, 'click_command': None, 'side': 'left', 'num': None}
+        default_args = {'width': 100, 'height': 50, 'border_color': '#37373D', 'text': 'Compile', 'socket_radius': 8, 'justify': 'center',
+                        'corner_radius': 25, 'x': None, 'y': None, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white',
+                        'font': ('', 10), 'highlightcolor': '#52d66c', 'hover': True, 'socket_hover': True, 'socket_color': 'green',
+                        'socket_hover_color': 'grey50', 'show_value': True, 'command': None, 'click_command': None, 'side': 'left', 'num': None}
         
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("command")
         args.pop("x")
         args.pop("y")
```

### Comparing `tknodesystem-0.4/tknodesystem/node_canvas.py` & `tknodesystem-0.5/tknodesystem/node_canvas.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/tknodesystem/node_menu.py` & `tknodesystem-0.5/tknodesystem/node_menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         else:
             self.attributes("-type", "splash")
             self.transparent_color = '#000001'
             self.corner = 0
             self.padding = 20
             self.attach.bind("<Double-Button-3>", self.popup, add="+")
             self.bind("<FocusOut>", lambda e: self._withdraw())
-            
+
         self.fg_color = customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"] if fg_color is None else fg_color
         self.scroll_button_color = customtkinter.ThemeManager.theme["CTkScrollbar"]["button_color"] if scrollbar_button_color is None else scrollbar_button_color
         self.scroll_hover_color = customtkinter.ThemeManager.theme["CTkScrollbar"]["button_hover_color"] if scrollbar_button_hover_color is None else scrollbar_button_hover_color
         self.border_color = customtkinter.ThemeManager.theme["CTkFrame"]["border_color"] if border_color is None else border_color
         self.button_color = customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"] if button_color is None else button_color
         self.text_color = customtkinter.ThemeManager.theme["CTkLabel"]["text_color"] if text_color is None else text_color
         
@@ -188,15 +188,16 @@
                 self.no_match.pack_forget()
             self.button_num = i
             
         else:
             self.no_match.pack_forget()
             for key in self.node.keys():
                 self.node[key].pack(fill="x", pady=5, padx=(self.padding,0))
-           
+        self.frame._parent_canvas.yview_moveto(0.0)
+        
     def _deiconify(self):
         if self.button_num>0:
             self.deiconify()
         
     def popup(self, event):
         if self.disable: return
         self._iconify(event.x_root, event.y_root)
```

### Comparing `tknodesystem-0.4/tknodesystem/node_types.py` & `tknodesystem-0.5/tknodesystem/node_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import __main__
 from .node import Node
 from .node_socket import NodeSocket
 from .node_args import Args
+import warnings
 
 class NodeValue(Node):
     def __init__(self, canvas, width=100, height=50, value=0, border_color='white', text=None, corner_radius=25,
                  border_width=0, fg_color='#37373D', text_color='white', font=("",10), socket_radius=8, socket_hover=True,
-                 socket_color="green", socket_hover_color="grey50", highlightcolor='#52d66c', hover=True,
+                 socket_color="green", socket_hover_color="grey50", highlightcolor='#52d66c', hover=True, justify="center",
                  click_command=None, side="right", x=0, y=0, num=None):
 
         self.text = text
         self.canvas = canvas
         
         self.args = Args.value_args(locals())
         
         if click_command:
             if click_command!="<lambda>":
                 if type(click_command) is str:
                     click_command = getattr(__main__, click_command)
                 self.args.update({"click_command": click_command.__name__})
             else:
                 click_command = None
-                print("Warning: currently <lamba function> cannot be saved and loaded, please use local function instead")
+                warnings.warn("Warning: currently <lamba function> cannot be saved and loaded, please use any local function instead")
             
         if self.text is None:
             self.text = f"Input{self.canvas.input_num}"
             
         self.canvas.input_num +=1
         self.connected_func = set()
         self.value = value
@@ -33,15 +34,15 @@
         
         if border_width==0:
             border_color = fg_color
 
         
         super().__init__(canvas=canvas, width=width, height=height, center=(width,height), text=str(self.text),
                          border_width=border_width, border_color=border_color, fg_color=fg_color, corner_radius=corner_radius,
-                         text_color=text_color, font=font, highlightcolor=highlightcolor, hover=hover,
+                         text_color=text_color, font=font, highlightcolor=highlightcolor, hover=hover, justify=justify,
                          click_command=click_command)
 
         if side=="left":
             center = (width-(width/2),height)
         else:
             center = (width+(width/2),height)
             
@@ -132,69 +133,73 @@
         if "socket_hover" in kwargs:
             self.output_.configure(hover=kwargs.pop("socket_hover"))
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
 
 class NodeOperation(Node):
-    def __init__(self, canvas, width=100, height=None, inputs=2, border_color='white', text=None,
+    def __init__(self, canvas, width=100, height=None, inputs=2, border_color='white', text=None, justify="center", hover_text=None,
                  socket_radius=8, corner_radius=25, border_width=0, fg_color='#37373D', text_color='white', font=("",10),
                  highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=0, y=0, none_inputs=False,
                  multiside=False, command=None, output_socket_color="green", click_command=None, socket_hover=True, num=None):
 
         self.text = text
         self.canvas = canvas
         self.type = 'NodeOperation'
+        self.hover_text = {} if hover_text is None else hover_text
         
         if self.text is None:
             self.text = f"Function{self.canvas.operation_num}"
             
         self.canvas.operation_num +=1
 
         if border_width==0:
             border_color = fg_color
-            
-        self.args = Args.func_args(locals())
-        
+
+        args = locals()
+        args['hover_text'] = self.hover_text
+        self.args = Args.func_args(args)
+
         if command:
             if command!="<lambda>":            
                 if type(command) is str:
                     command = getattr(__main__, command)
                 self.args.update({"command": command.__name__})
             else:
                 command = None
-                print("Warning: currently <lamba function> cannot be saved and loaded, please use local function instead")
+                warnings.warn("Warning: currently <lamba function> cannot be saved and loaded, please use any local function instead")
         if click_command:
             if click_command!="<lambda>":
                 if type(click_command) is str:
                     click_command = getattr(__main__, click_command)
                 self.args.update({"click_command": click_command.__name__})
             else:
                 click_command = None
-                print("Warning: currently <lamba function> cannot be saved and loaded, please use local function instead")
+                warnings.warn("Warning: currently <lamba function> cannot be saved and loaded, please use any local function instead")
                 
         self.command = command
         
         if height is None:
             height = 50 + (inputs*10)
             
-        super().__init__(canvas=canvas, width=width, height=height, center=(width,height), 
+        super().__init__(canvas=canvas, width=width, height=height, center=(width,height), justify=justify,
                          border_width=border_width, fg_color=fg_color, border_color=border_color,
                          text_color=text_color, font=font, click_command=click_command, corner_radius=corner_radius,
                          highlightcolor=highlightcolor, text=str(self.text), hover=hover)
 
         self.line1 = None
         self.line2 = None
         self.line3 = None
         self.line4 = None
         self.line5 = None
         self.socket_colors = []
         self.connected_node = set()
         self.connected_node_first = None
         self.none_values = none_inputs
+        
         x_pos = x
         y_pos = y
             
         if type(socket_color) is list:
             self.socket_colors = socket_color
         else:
             for i in range(5):
@@ -231,15 +236,15 @@
                                   fg_color=output_socket_color, hover_color=socket_hover_color, socket_num=num[0] if num else None,
                                   border_width=border_width, border_color=border_color, hover=socket_hover)
         self.canvas.tag_bind(self.output_.ID, '<Button-1>', self.connect_output)
         self.socket_nums.append(self.output_.socket_num)
         
         center = (width/2, y * x + height/2)     
         self.input_1 = NodeSocket(canvas, radius=socket_radius, center=center, fg_color=self.socket_colors[0],
-                                  hover_color=socket_hover_color, border_width=border_width,
+                                  hover_color=socket_hover_color, border_width=border_width, hover=socket_hover,
                                   border_color=border_color, socket_num=num[1] if num else None)
         
         id_list = [self.output_.ID, self.input_1.ID]
         self.canvas.tag_bind(self.input_1.ID, '<Button-1>', lambda e: self.connect_input(self.line1,'input1'))
         self.socket_nums.append(self.input_1.socket_num)
         
         if self.inputs>=2:
@@ -289,15 +294,18 @@
             id_list.append(self.input_5.ID)
             self.socket_nums.append(self.input_5.socket_num)
             
         self.allIDs = self.allIDs + id_list
         self.bind_all_to_movement()
         self.id_list = id_list
         self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
-   
+
+        for i in self.hover_text:
+            self.config_socket(**self.hover_text[i])
+       
         for j in range(self.canvas.gain_in):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 0.9, 0.9)
@@ -474,15 +482,52 @@
                 i.update()
                 
     def exists(self):
         if self.ID in self.canvas.find_all():
             return True
         else:
             return False
-        
+
+    def config_socket(self, index: int, hover_text: str=None, hover_text_color=None, hover_bg=None, **kwargs):
+        if index==1:
+            socket = self.input_1
+        elif index==2:
+            socket = self.input_2
+        elif index==3:
+            socket = self.input_3
+        elif index==4:
+            socket = self.input_4
+        elif index==5:
+            socket = self.input_5
+        else:
+            return
+
+        kwarg_args = {}
+        for i in kwargs:
+            kwarg_args  = {i: kwargs[i]}
+            
+        self.hover_text[str(index)] = {'index': index, 'hover_text': hover_text, 'hover_text_color': hover_text_color, 'hover_bg': hover_bg, **kwarg_args}
+
+        if hover_text:
+            socket.hover_message = True
+            socket.msg.set(hover_text)
+        else:
+            socket.hover_message = False
+            
+        if hover_text_color:
+            socket.hover_text.configure(fg=hover_text_color)
+            
+        if hover_bg:
+            socket.hover_text.configure(bg=hover_bg)
+            
+        if "socket_color" in kwargs:
+            socket.configure(fg_color=kwargs.pop("socket_color"))
+
+        self.configure(**kwargs)
+            
     def configure(self, **kwargs):
         """ configure options """
         
         if "text" in kwargs:
             self.text = kwargs.pop("text")
             super().configure(text=self.text)
         if "fg_color" in kwargs:
@@ -540,15 +585,15 @@
                 self.input_5.configure(hover=hover)
             except: None
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
         
 class NodeCompile(Node):
-    def __init__(self, canvas, width=100, height=50, border_color='white', text="Compile", socket_radius=8, corner_radius=25, x=0, y=0,
+    def __init__(self, canvas, width=100, height=50, border_color='white', text="Compile", socket_radius=8, corner_radius=25, x=0, y=0, justify="center",
                  border_width=0, fg_color='#37373D',text_color='white', font=("",10), highlightcolor='#52d66c', hover=True, socket_hover=True,
                  socket_color="green", socket_hover_color="grey50", show_value=True, command=None, click_command=None, side="left", num=None):
 
         self.canvas = canvas
         self.text = text
         self.type = 'NodeCompile'
         
@@ -562,26 +607,26 @@
         if command:
             if command!="<lambda>":            
                 if type(command) is str:
                     command = getattr(__main__, command)
                 self.args.update({"command": command.__name__})
             else:
                 command = None
-                print("Warning: currently <lamba function> cannot be saved and loaded, please use local function instead")
+                warnings.warn("Warning: currently <lamba function> cannot be saved and loaded, please use any local function instead")
         if click_command:
             if click_command!="<lambda>":
                 if type(click_command) is str:
                     click_command = getattr(__main__, click_command)
                 self.args.update({"click_command": click_command.__name__})
             else:
                 click_command = None
-                print("Warning: currently <lamba function> cannot be saved and loaded, please use local function instead")
+                warnings.warn("Warning: currently <lamba function> cannot be saved and loaded, please use any local function instead")
                 
         super().__init__(canvas=canvas, width=width, height=height, center=(width,height), text=str(text), corner_radius=corner_radius,
-                         border_width=border_width, fg_color=fg_color, border_color=border_color, hover=hover,
+                         border_width=border_width, fg_color=fg_color, border_color=border_color, hover=hover, justify=justify,
                          text_color=text_color, font=font, click_command=click_command, highlightcolor=highlightcolor)
 
         self.line1 = None
         self.line2 = None
         self.cellinput1 = None
         self.cellinput2 = None
         self.celloutput = None
```

### Comparing `tknodesystem-0.4/tknodesystem/node_wire.py` & `tknodesystem-0.5/tknodesystem/node_wire.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.4/tknodesystem.egg-info/PKG-INFO` & `tknodesystem-0.5/tknodesystem.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.4
+Version: 0.5
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
-Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
+Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes,visual-scripting
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -19,15 +19,15 @@
 
 ## Feature
 - Lightweight library
 - Easy to install and use
 - Multiple nodes and inputs
 - **Save/Load** node trees
 - Canvas with **drag and zoom** ability
-- Customizable options
+- Customizable nodes and options
 - Built-in **Node menu**
 
 ## Installation
 ```
 pip install tknodesystem
 ```
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/TkNodeSystem?&color=cyan&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/TkNodeSystem/archive/refs/heads/main.zip)
@@ -56,14 +56,14 @@
 
 ## Documentation
 Full documentation can be found in the **Wiki** page
 
 [<img src="https://img.shields.io/badge/View-Docs-informational?&color=c8ab09&style=for-the-badge" width="150">](https://github.com/Akascape/TkNodeSystem/wiki)
 
 ## Examples
-Examples are given in the `examples` folder
+Examples are given in the [`examples`](https://github.com/Akascape/TkNodeSystem/tree/main/examples) folder
 ![Example App](https://github.com/Akascape/TkNodeSystem/assets/89206401/ea818333-c979-4402-bc7c-8850930dc087)
 
 ### Bug Fixes
 This library is at **experimental stage**, so there must be some bugs which can appear randomly.
 
 **So, please report the bugs at the issues/discussions tab. A pull request is always welcomed :)**
```

### Comparing `tknodesystem-0.4/tknodesystem.egg-info/SOURCES.txt` & `tknodesystem-0.5/tknodesystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

