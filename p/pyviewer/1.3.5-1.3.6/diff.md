# Comparing `tmp/pyviewer-1.3.5.tar.gz` & `tmp/pyviewer-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviewer-1.3.5.tar", last modified: Thu May 25 14:49:34 2023, max compression
+gzip compressed data, was "pyviewer-1.3.6.tar", last modified: Thu Jun  1 02:37:49 2023, max compression
```

## Comparing `pyviewer-1.3.5.tar` & `pyviewer-1.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:34.541093 pyviewer-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-05-25 14:49:23.000000 pyviewer-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 14:49:34.541093 pyviewer-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-25 14:49:23.000000 pyviewer-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:34.541093 pyviewer-1.3.5/pyviewer/
--rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/MPLUSRounded1c-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/easy_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/gl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/imgui_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/params.py
--rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/roboto_mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/single_image_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/toolbar_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-25 14:49:23.000000 pyviewer-1.3.5/pyviewer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:49:34.541093 pyviewer-1.3.5/pyviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-25 14:49:34.000000 pyviewer-1.3.5/pyviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 14:49:34.000000 pyviewer-1.3.5/pyviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:49:34.000000 pyviewer-1.3.5/pyviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 14:49:34.000000 pyviewer-1.3.5/pyviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 14:49:34.000000 pyviewer-1.3.5/pyviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:49:34.541093 pyviewer-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 14:49:23.000000 pyviewer-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:49.180807 pyviewer-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-06-01 02:37:41.000000 pyviewer-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-01 02:37:49.180807 pyviewer-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-01 02:37:41.000000 pyviewer-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:49.180807 pyviewer-1.3.6/pyviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)  3423528 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/MPLUSRounded1c-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/easy_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/gl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/imgui_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71936 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/roboto_mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/single_image_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/toolbar_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-06-01 02:37:41.000000 pyviewer-1.3.6/pyviewer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:37:49.180807 pyviewer-1.3.6/pyviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-01 02:37:49.000000 pyviewer-1.3.6/pyviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-01 02:37:49.000000 pyviewer-1.3.6/pyviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:37:49.000000 pyviewer-1.3.6/pyviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 02:37:49.000000 pyviewer-1.3.6/pyviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 02:37:49.000000 pyviewer-1.3.6/pyviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:37:49.180807 pyviewer-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-01 02:37:41.000000 pyviewer-1.3.6/setup.py
```

### Comparing `pyviewer-1.3.5/LICENSE` & `pyviewer-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/PKG-INFO` & `pyviewer-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.5
+Version: 1.3.6
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.5/README.md` & `pyviewer-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/MPLUSRounded1c-Medium.ttf` & `pyviewer-1.3.6/pyviewer/MPLUSRounded1c-Medium.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/gl_viewer.py` & `pyviewer-1.3.6/pyviewer/gl_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/imgui_themes.py` & `pyviewer-1.3.6/pyviewer/imgui_themes.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/params.py` & `pyviewer-1.3.6/pyviewer/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import imgui
 from pyviewer.utils import enum_slider, combo_box_vals, slider_range_int, slider_range_float, strict_dataclass
+from typing import Tuple
 
 """ Small param wrappers for automatically creating UI widgets """
 
 class Param:
     def __init__(self, type, label: str, default_val, tooltip: str = None) -> None:
         self.type = type
         self.label = label
@@ -75,16 +76,16 @@
             imgui.same_line()
             if imgui.button(f'>##{self.label}'):
                 changed, val = (True, max(self.min, min(self.max, val + 1)))
 
         return changed, val
 
 class Int2Param(_Range2Param):
-    def __init__(self, label, default_val: tuple[int], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
-        super().__init__(tuple[int], label, default_val, minval, maxval, overlap, tooltip)
+    def __init__(self, label, default_val: Tuple[int], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
+        super().__init__(Tuple[int], label, default_val, minval, maxval, overlap, tooltip)
     
     def draw_widget(self):
         if not self.overlap:
             return slider_range_int(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_int2(self.label, *self.value, self.min, self.max)
 
@@ -92,16 +93,16 @@
     def __init__(self, label, default_val: float, minval, maxval, tooltip: str = None) -> None:
         super().__init__(float, label, default_val, minval, maxval, tooltip)
     
     def draw_widget(self):
         return imgui.slider_float(self.label, self.value, self.min, self.max)
     
 class Float2Param(_Range2Param):
-    def __init__(self, label, default_val: tuple[float], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
-        super().__init__(tuple[float], label, default_val, minval, maxval, overlap, tooltip)
+    def __init__(self, label, default_val: Tuple[float], minval, maxval, overlap: bool = True, tooltip: str = None) -> None:
+        super().__init__(Tuple[float], label, default_val, minval, maxval, overlap, tooltip)
     
     def draw_widget(self):
         if not self.overlap:
             return slider_range_float(*self.value, self.min, self.max, title=self.label)
         else:
             return imgui.slider_float2(self.label, *self.value, self.min, self.max)
```

### Comparing `pyviewer-1.3.5/pyviewer/roboto_mono.ttf` & `pyviewer-1.3.6/pyviewer/roboto_mono.ttf`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/single_image_viewer.py` & `pyviewer-1.3.6/pyviewer/single_image_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/toolbar_viewer.py` & `pyviewer-1.3.6/pyviewer/toolbar_viewer.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer/utils.py` & `pyviewer-1.3.6/pyviewer/utils.py`

 * *Files identical despite different names*

### Comparing `pyviewer-1.3.5/pyviewer.egg-info/PKG-INFO` & `pyviewer-1.3.6/pyviewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviewer
-Version: 1.3.5
+Version: 1.3.6
 Summary: Interactyive python viewers
 Home-page: https://github.com/harskish/pyviewer
 Author: Erik Härkönen
 Author-email: erik.harkonen@hotmail.com
 License: CC BY-NC-SA 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyviewer-1.3.5/setup.py` & `pyviewer-1.3.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 from pathlib import Path
 
 import sys
 if 'develop' in sys.argv:
     print("WARNING: 'python setup.py develop' won't install \
         dependencies correctly, please use 'pip install -e .' instead.")
 
+# Workflow:
+# Increment version number (together with other changes)
+# git commit
+# git tag -a "vX.X.X" -m "vX.X.X"  (only annotated tags show up in GitHub)
+# git push --follow-tags
 setup(name='pyviewer',
-    version='1.3.5',
+    version='1.3.6',
     description='Interactyive python viewers',
     author='Erik Härkönen',
     author_email='erik.harkonen@hotmail.com',
     url='https://github.com/harskish/pyviewer',
     packages=['pyviewer'], # name of importable thing
     setup_requires=['wheel'],
     install_requires=[
```

