# Comparing `tmp/cwapi3d-2.0.4.tar.gz` & `tmp/cwapi3d-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-2.0.4.tar", last modified: Thu May 18 14:18:54 2023, max compression
+gzip compressed data, was "cwapi3d-2.0.6.tar", last modified: Thu Jun  1 15:30:51 2023, max compression
```

## Comparing `cwapi3d-2.0.4.tar` & `cwapi3d-2.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (123)    86279 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/cadwork/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-18 14:18:53.000000 cwapi3d-2.0.4/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.995065 cwapi3d-2.0.4/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    33675 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 14:18:53.999065 cwapi3d-2.0.4/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-18 14:18:40.000000 cwapi3d-2.0.4/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    89894 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/cadwork/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    34859 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-2.0.4/LICENSE` & `cwapi3d-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/PKG-INFO` & `cwapi3d-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.4
+Version: 2.0.6
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.4/README.md` & `cwapi3d-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/setup.py` & `cwapi3d-2.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cwapi3d',
-    version='2.0.4',
+    version='2.0.6',
     author='Cadwork',
     author_email='it@cadwork.ca',
     description='Python bindings for CwAPI3D',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cwapi3d/cwapi3dpython',
     classifiers=[
```

### Comparing `cwapi3d-2.0.4/src/attribute_controller/__init__.pyi` & `cwapi3d-2.0.6/src/attribute_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/bim_controller/__init__.pyi` & `cwapi3d-2.0.6/src/bim_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/cadwork/__init__.pyi` & `cwapi3d-2.0.6/src/cadwork/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2359,87 +2359,256 @@
 # Node Symbols
 
 
 @unique
 class node_symbol(Enum):
     """Change node symbol. 
 
+    Examples:
+        >>> point = cadwork.point_3d(0, 0, 0)
+        >>> node = element_controller.create_node(point)
+        >>> node.set_node_symbol(node, node_symbol.circle)
+
     Args:
-        Enum (int): symbol type
+        small_circle (int): 1
+        square (int): 2
+        cross (int): 3
+        circle (int): 4
+        filled_circle (int): 5
+        chess_square (int): 6
+        half_filled_square (int): 7
+        cross_square (int): 8
+        filled_square (int): 9       
     """
-    SmallSquare = 1
-    Square = 2
-    Cross = 3
-    Circle = 4
-    FilledCircle = 5
-    ChessSquare = 6
-    HalfFilledSquare = 7
-    CrossSquare = 8
-    FilledSquare = 9
+    small_circle = 1
+    square = 2
+    cross = 3
+    circle = 4
+    filled_circle = 5
+    chess_square = 6
+    half_filled_square = 7
+    cross_square = 8
+    filled_square = 9
+
+    def __int__(self) -> None:
+        return self.value
 
 
 @unique
 class element_module_detail(Enum):
     """Add element situation to detail. 
 
+    Examples:
+        >>> element_controller.add_elements_to_detail(element_ids, element_module_detail.cross)
+
     Args:
-        Enum (int): detail situation
+        none (int): 0
+        angle (int): 1
+        area (int): 2
+        cross (int): 3
+        edge (int): 4
+        end (int): 5
+        line (int): 6
+        open (int): 7
+        t_connection (int): 8
+        floor_area (int): 9
+        floor_end (int): 10
+        floor_line (int): 11
+        floor_open (int): 12
+
     """
-    no_detail = 0
-    angle_detail = 1
-    area_detail = 2
-    cross_detail = 3
-    edge_detail = 4
-    end_detail = 5
-    line_detail = 6
-    open_detail = 7
-    t_detail = 8
-    floor_area_detail = 10
-    floor_end_detail = 11
-    floor_line_detail = 12
-    floor_open_detail = 13
+    none_ = 0,
+    angle = 1,
+    area = 2,
+    cross = 3,
+    edge = 4,
+    end = 5,
+    line = 6,
+    open = 7,
+    t_connection = 8,
+    floor_area = 9,
+    floor_end = 10,
+    floor_line = 11,
+    floor_open = 12
+
+    def __int__(self) -> None:
+        return self.value
 
 
 @unique
 class division_zone_direction(Enum):
     """ Add division zone direction.
 
+    Examples:
+        >>> point = cadwork.point_3d(0, 0, 0)
+        >>> geometry_controller.create_division_zone(123456, point, division_zone_direction.positive)
+
     Args:
-        Enum (int): direction
+        positive (int): 1
+        negative (int): -1
+        none (int): 0
     """
     positive = 1
     negative = -1
     none = 0
 
+    def __int__(self) -> None:
+        return self.value
+
 
 @unique
 class shortcut_key(Enum):
     """Shortcut key.
 
+    Examples:
+        >>> utility_controller.execute_shortcut(shortcut_key.F1, shortcut_key_modifier.shift)
+
     Args:
-        Enum (int): key
+        F1 (int): 1
+        F2 (int): 2
+        F3 (int): 3
+        F4 (int): 4
+        F5 (int): 5
+        F6 (int): 6
+        F7 (int): 7
+        F8 (int): 8
+        F9 (int): 9
+        F10 (int): 10
+        F11 (int): 11
+        F12 (int): 12
     """
     F1 = 1
     F2 = 2
     F3 = 3
     F4 = 4
     F5 = 5
     F6 = 6
     F7 = 7
     F8 = 8
     F9 = 9
     F10 = 10
     F11 = 11
     F12 = 12
 
+    def __int__(self) -> None:
+        return self.value
+
 
 @unique
 class shortcut_key_modifier(Enum):
     """Shortcut key.
 
+    Examples:
+        >>> utility_controller.execute_shortcut(shortcut_key.F1, shortcut_key_modifier.shift)
+
     Args:
-        Enum (int): key
+        none (int): 0
+        shift (int): 1
+        ctrl (int): 2
+        alt (int): 3
     """
     none = 0
     shift = 1
     ctrl = 2
     alt = 3
+
+    def __int__(self) -> None:
+        return self.value
+
+
+@unique
+class btl_version(Enum):
+    """BTL version.
+
+    Examples:
+        >>> machine_controller.export_btl(btl_version.btl_1_6, "C:\\temp\\test.btl")
+
+    Args:
+        btl_1_0 (int): 110
+        btl_1_1 (int): 111
+        btl_1_2 (int): 112
+        btl_1_3 (int): 113
+        btl_1_4 (int): 114
+        btl_1_5 (int): 115
+        btl_1_6 (int): 116
+
+    """
+    btl_1_0 = 110
+    btl_1_1 = 111
+    btl_1_2 = 112
+    btl_1_3 = 113
+    btl_1_4 = 114
+    btl_1_5 = 115
+    btl_1_6 = 116
+
+    def __int__(self) -> None:
+        return self.value
+
+
+@unique
+class hundegger_machine_type(Enum):
+    """Hundegger machine type.
+
+    Examples:
+        >>> machine_controller.export_hundegger(hundegger_machine_type.k2)
+
+    Args:
+        p8_10 (int): 1
+        k1 (int): 2
+        k2 (int): 3
+        k2_cambium (int): 4
+        k2_uf_5 (int): 5
+        k2_uf_5_cambium (int): 6
+        speedcut (int): 7
+        pba (int): 8
+        pba_bvx (int): 9
+        pba_bvx_cambium (int): 10
+        spm (int): 12
+        spm_cambium (int): 13
+        robot_drive (int): 14
+        turbo_drive (int): 15
+
+    """
+
+    p8_10 = 1
+    k1 = 2
+    k2 = 3
+    k2_cambium = 4
+    k2_uf_5 = 5
+    k2_uf_5_cambium = 6
+    speedcut = 7
+    pba = 8
+    pba_bvx = 9
+    pba_bvx_cambium = 10
+    spm = 12
+    spm_cambium = 13
+    robot_drive = 14
+    turbo_drive = 15
+
+    def __int__(self) -> None:
+        return self.value
+
+
+@unique
+class weinmann_mfb_version(Enum):
+    """Weinmann MFB version.
+
+    Examples:
+        >>> machine_controller.export_weinmann_mfb(weinmann_mfb_version.wup_2_0)
+
+    Args:
+        wup_2_0 (int): 20
+        wup_3_1 (int): 31
+        wup_3_2 (int): 32
+        wup_3_3 (int): 33
+        wup_3_4 (int): 34
+
+    """
+
+    wup_2_0 = 20
+    wup_3_1 = 31
+    wup_3_2 = 32
+    wup_3_3 = 33
+    wup_3_4 = 34
+
+    def __int__(self) -> None:
+        return self.value
```

### Comparing `cwapi3d-2.0.4/src/connector_axis_controller/__init__.pyi` & `cwapi3d-2.0.6/src/connector_axis_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-2.0.6/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.4
+Version: 2.0.6
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.4/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-2.0.6/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/element_controller/__init__.pyi` & `cwapi3d-2.0.6/src/element_controller/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
+"""Provide several sample math calculations.
+
+This module allows the user to make mathematical calculations.
+
+The module contains the following functions:
+
+- `add(a, b)` - Returns the sum of two numbers.
+- `subtract(a, b)` - Returns the difference of two numbers.
+- `multiply(a, b)` - Returns the product of two numbers.
+- `divide(a, b)` - Returns the quotient of two numbers.
+"""
+
+
 from typing import List
 from cadwork import (element_module_properties,
                      point_3d,
-                     element_module_detail)
+                     )
 
 
 def get_all_identifiable_element_ids() -> List[int]:
     """get all identifiable element IDs (visible and unvisible)
 
     [:information_source: Available for script filled attributes](#){.mark-text}
 
@@ -1296,7 +1309,44 @@
         >>> element_ids = ec.get_active_identifiable_element_ids()
         >>> ec.move_element_with_undo(element_ids, gc.get_yl(*element_ids) * 1500.)
 
     Args:
         elements (List[int]): element IDs
         aVector (point_3d): a Target
     """
+
+
+def create_normal_axis_points(p1: point_3d, p2: point_3d) -> int:
+    """create normal axis points
+
+    Args:
+        p1 (point_3d): point 1
+        p2 (point_3d): point 2
+
+    Returns:
+        int: element ID
+    """
+
+
+def create_normal_axis_vectors(length: float, p1: point_3d, direction: point_3d) -> int:
+    """create normal axis vectors
+
+    Args:
+        length (float): length
+        p1 (point_3d): point 1
+        direction (point_3d): direction
+
+    Returns:
+        int: element ID
+    """
+
+
+def convert_bolt_to_standardconnector(elements: List[int], standard_connector_axis_name: str) -> int:
+    """convert bolt to standard connector
+
+    Args:
+        elements (List[int]): element IDs
+        standard_connector_axis_name (str): standard connector axis name
+
+    Returns:
+        int: element ID
+    """
```

### Comparing `cwapi3d-2.0.4/src/endtype_controller/__init__.pyi` & `cwapi3d-2.0.6/src/endtype_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/file_controller/__init__.pyi` & `cwapi3d-2.0.6/src/file_controller/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -237,7 +237,32 @@
 
 def get_blum_export_path() -> str:
     """Get blum export path
 
     Returns:
         str: file path
     """
+
+
+def import_element_light(file_path: str, insert_position: point_3d) -> int:
+    """Imports an element light
+        allowed formats are OBJ, SKP
+
+    Examples:
+    >>> import_element_light("C:\\UserXY\\Files\\example.obj", point_3d(0,0,0))
+
+    Args:
+        file_path (str): file path
+        insert_position (point_3d): insert position
+
+    Returns:
+        int: element ID
+    """
+
+
+def export_glb_file(elements: List[int], file: str) -> None:
+    """Exports a GLB file
+
+    Args:
+        elements (List[int]): element IDs
+        file (str): file path
+    """
```

### Comparing `cwapi3d-2.0.4/src/geometry_controller/__init__.pyi` & `cwapi3d-2.0.6/src/geometry_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/list_controller/__init__.pyi` & `cwapi3d-2.0.6/src/list_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/machine_controller/__init__.pyi` & `cwapi3d-2.0.6/src/machine_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/material_controller/__init__.pyi` & `cwapi3d-2.0.6/src/material_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/scene_controller/__init__.pyi` & `cwapi3d-2.0.6/src/scene_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-2.0.6/src/shop_drawing_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/utility_controller/__init__.pyi` & `cwapi3d-2.0.6/src/utility_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.4/src/visualization_controller/__init__.pyi` & `cwapi3d-2.0.6/src/visualization_controller/__init__.pyi`

 * *Files identical despite different names*

