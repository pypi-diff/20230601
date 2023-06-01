# Comparing `tmp/pginter-0.2.3.tar.gz` & `tmp/pginter-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pginter-0.2.3.tar", last modified: Wed May 31 21:17:26 2023, max compression
+gzip compressed data, was "pginter-0.2.4.tar", last modified: Thu Jun  1 19:06:29 2023, max compression
```

## Comparing `pginter-0.2.3.tar` & `pginter-0.2.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.610450 pginter-0.2.3/
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.3/LICENSE
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.3/MANIFEST.in
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 21:17:26.610450 pginter-0.2.3/PKG-INFO
--rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.3/README.md
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.3/pyproject.toml
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-05-31 21:17:26.610450 pginter-0.2.3/setup.cfg
--rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-05-31 21:17:03.000000 pginter-0.2.3/setup.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.603783 pginter-0.2.3/src/
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.603783 pginter-0.2.3/src/pginter/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.3/src/pginter/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20488 2023-05-31 20:25:21.000000 pginter-0.2.3/src/pginter/_pg_root.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.3/src/pginter/icon.png
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.607117 pginter-0.2.3/src/pginter/theme/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.3/src/pginter/theme/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.3/src/pginter/theme/_manager.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.607117 pginter-0.2.3/src/pginter/theme/themes/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.3/src/pginter/theme/themes/default.json
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.607117 pginter-0.2.3/src/pginter/types/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.3/src/pginter/types/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.3/src/pginter/types/_better_dict.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.3/src/pginter/types/_binds.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.3/src/pginter/types/_color.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.3/src/pginter/types/_constants.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.3/src/pginter/types/_geo_types.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.3/src/pginter/types/_notifications.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.3/src/pginter/types/_scheme.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.3/src/pginter/types/_style.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.3/src/pginter/types/_tk_vars.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.607117 pginter-0.2.3/src/pginter/utils/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.3/src/pginter/utils/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.3/src/pginter/utils/_funcs.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.610450 pginter-0.2.3/src/pginter/widgets/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.3/src/pginter/widgets/__init__.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.3/src/pginter/widgets/_button.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.3/src/pginter/widgets/_entry.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26515 2023-05-31 20:53:29.000000 pginter-0.2.3/src/pginter/widgets/_frame.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-05-31 20:24:58.000000 pginter-0.2.3/src/pginter/widgets/_geo_manager.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.3/src/pginter/widgets/_label.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.3/src/pginter/widgets/_supports_children.py
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.3/src/pginter/widgets/_surface_frame.py
-drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-05-31 21:17:26.603783 pginter-0.2.3/src/pginter.egg-info/
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-05-31 21:17:26.000000 pginter-0.2.3/src/pginter.egg-info/PKG-INFO
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-05-31 21:17:26.000000 pginter-0.2.3/src/pginter.egg-info/SOURCES.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-05-31 21:17:26.000000 pginter-0.2.3/src/pginter.egg-info/dependency_links.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-05-31 21:17:26.000000 pginter-0.2.3/src/pginter.egg-info/requires.txt
--rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-05-31 21:17:26.000000 pginter-0.2.3/src/pginter.egg-info/top_level.txt
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.790060 pginter-0.2.4/
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)     1065 2023-02-04 21:58:18.000000 pginter-0.2.4/LICENSE
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      115 2023-05-31 20:31:36.000000 pginter-0.2.4/MANIFEST.in
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-01 19:06:29.790060 pginter-0.2.4/PKG-INFO
+-rwxrwxrwx   0 nilusink  (1000) nilusink  (1000)       54 2023-02-04 21:58:18.000000 pginter-0.2.4/README.md
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)      116 2023-05-24 18:38:46.000000 pginter-0.2.4/pyproject.toml
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       38 2023-06-01 19:06:29.790060 pginter-0.2.4/setup.cfg
+-rwxr-xr-x   0 nilusink  (1000) nilusink  (1000)     1021 2023-05-31 21:17:56.000000 pginter-0.2.4/setup.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.780060 pginter-0.2.4/src/
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.780060 pginter-0.2.4/src/pginter/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      124 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    21906 2023-06-01 19:00:08.000000 pginter-0.2.4/src/pginter/_pg_root.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    20019 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/icon.png
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter/theme/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       35 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/theme/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     3997 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/theme/_manager.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter/theme/themes/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      663 2023-05-25 20:39:17.000000 pginter-0.2.4/src/pginter/theme/themes/default.json
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.786726 pginter-0.2.4/src/pginter/types/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      335 2023-05-25 22:58:36.000000 pginter-0.2.4/src/pginter/types/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      368 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/types/_better_dict.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      455 2023-05-25 19:05:55.000000 pginter-0.2.4/src/pginter/types/_binds.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4227 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/types/_color.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      456 2023-05-25 23:31:05.000000 pginter-0.2.4/src/pginter/types/_constants.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      273 2023-05-14 20:36:55.000000 pginter-0.2.4/src/pginter/types/_geo_types.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      161 2023-05-25 15:16:09.000000 pginter-0.2.4/src/pginter/types/_notifications.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5384 2023-05-30 12:53:46.000000 pginter-0.2.4/src/pginter/types/_scheme.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     6528 2023-05-15 19:07:58.000000 pginter-0.2.4/src/pginter/types/_style.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4301 2023-05-25 23:22:37.000000 pginter-0.2.4/src/pginter/types/_tk_vars.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.786726 pginter-0.2.4/src/pginter/utils/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       49 2023-05-14 20:09:36.000000 pginter-0.2.4/src/pginter/utils/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      872 2023-05-25 23:31:06.000000 pginter-0.2.4/src/pginter/utils/_funcs.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.790060 pginter-0.2.4/src/pginter/widgets/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      197 2023-05-25 22:58:36.000000 pginter-0.2.4/src/pginter/widgets/__init__.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     4982 2023-05-25 10:36:44.000000 pginter-0.2.4/src/pginter/widgets/_button.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    14178 2023-05-30 19:45:06.000000 pginter-0.2.4/src/pginter/widgets/_entry.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26515 2023-05-31 20:53:29.000000 pginter-0.2.4/src/pginter/widgets/_frame.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)    26315 2023-06-01 18:54:30.000000 pginter-0.2.4/src/pginter/widgets/_geo_manager.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     5961 2023-05-30 19:49:43.000000 pginter-0.2.4/src/pginter/widgets/_label.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      412 2023-02-10 14:14:25.000000 pginter-0.2.4/src/pginter/widgets/_supports_children.py
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1022 2023-05-24 20:39:09.000000 pginter-0.2.4/src/pginter/widgets/_surface_frame.py
+drwxr-xr-x   0 nilusink  (1000) nilusink  (1000)        0 2023-06-01 19:06:29.783393 pginter-0.2.4/src/pginter.egg-info/
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)      493 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/PKG-INFO
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)     1028 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/SOURCES.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        1 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/dependency_links.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)       33 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/requires.txt
+-rw-r--r--   0 nilusink  (1000) nilusink  (1000)        8 2023-06-01 19:06:29.000000 pginter-0.2.4/src/pginter.egg-info/top_level.txt
```

### Comparing `pginter-0.2.3/LICENSE` & `pginter-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/setup.py` & `pginter-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pginter",
-    version="0.2.3",
+    version="0.2.4",
     author="Nilusink",
     author_email="nilusink@protonmail.com",
     description="A python GUI interface, based on pygame",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Nilusink/PgInter",
     # project_urls={
```

### Comparing `pginter-0.2.3/src/pginter/_pg_root.py` & `pginter-0.2.4/src/pginter/_pg_root.py`

 * *Files 12% similar despite different names*

```diff
@@ -114,14 +114,44 @@
     def mouse_pos(self) -> tuple[int, int]:
         return self._mouse_pos
 
     @property
     def root(self) -> tp.Self:
         return self
 
+    @property
+    def _height_configured(self) -> bool:
+        return True
+
+    @property
+    def _width_configured(self) -> bool:
+        return True
+
+    @property
+    def _height(self) -> int:
+        return pg.display.get_window_size()[1]
+
+    @_height.setter
+    def _height(self, *_) -> None:
+        """
+        value should not be set, but no error should occur
+        """
+        pass
+
+    @property
+    def _width(self) -> int:
+        return pg.display.get_window_size()[0]
+
+    @_width.setter
+    def _width(self, *_) -> None:
+        """
+        value should not be set, but no error should occur
+        """
+        pass
+
     def get_focus(self) -> GeometryManager | None:
         """
         get the currently focused item
         """
         return self._focus_item
 
     def set_focus(
@@ -242,299 +272,299 @@
         """
         while self._running:
             self.update_idletasks()
             self.update()
 
             self._clk.tick(self._max_framerate)
 
-    def calculate_geometry(self):
-        """
-        calculate how each individual child should be placed
-        """
-        match self._layout:
-            case Layout.Absolute:  # Absolute
-                # since the positioning is absolute, the children should not influence the parents size
-                for child, params in self._child_params:
-                    child.set_position(params.x, params.y)
-
-                return
-
-            case Layout.Pack:
-                directional_dict: dict[str, int | list] = {"total_x": 0, "total_y": 0, "children": [], "sizes": []}
-                top = deepcopy(directional_dict)
-                bottom = deepcopy(directional_dict)
-                left = deepcopy(directional_dict)
-                right = deepcopy(directional_dict)
-
-                # get all sizes and group by anchor
-                for child, param in self._child_params:
-                    child_size = child.calculate_size()
-
-                    if param.anchor == TOP:
-                        top["children"].append(child)
-                        top["sizes"].append(child_size)
-                        top["total_x"] += child_size[0]
-                        top["total_y"] += child_size[1]
-
-                    elif param.anchor == BOTTOM:
-                        bottom["children"].append(child)
-                        bottom["sizes"].append(child_size)
-                        bottom["total_x"] += child_size[0]
-                        bottom["total_y"] += child_size[1]
-
-                    elif param.anchor == LEFT:
-                        left["children"].append(child)
-                        left["sizes"].append(child_size)
-                        left["total_x"] += child_size[0]
-                        left["total_y"] += child_size[1]
-
-                    elif param.anchor == RIGHT:
-                        right["children"].append(child)
-                        right["sizes"].append(child_size)
-                        right["total_x"] += child_size[0]
-                        right["total_y"] += child_size[1]
-
-                top["total_y"] += self._layout_params.padding * len(top["children"]) - 1
-                bottom["total_y"] += self._layout_params.padding * len(bottom["children"]) - 1
-
-                left["total_x"] += self._layout_params.padding * len(left["children"]) - 1
-                right["total_x"] += self._layout_params.padding * len(right["children"]) - 1
-
-                min_x = max([top["total_x"], bottom["total_x"], left["total_x"] + right["total_x"]])
-                min_y = max([left["total_y"], right["total_y"], top["total_y"] + bottom["total_y"]])
-
-                # add margin
-                min_x += self.layout_params.margin * 2
-                min_y += self.layout_params.margin * 2
-
-                self._min_size = min_x, min_y
-
-                total_x, total_y = self.calculate_size()
-
-                # tell the children where they should be
-                y_cen = total_y / 2
-                x_cen = total_x / 2
-
-                # left
-                x_now = self._layout_params.margin
-                for child, size in zip(left["children"], left["sizes"]):
-                    child.set_position(x_now, y_cen - size[1] / 2)
-                    x_now += size[0] + self._layout_params.padding
-
-                    # right
-                x_now = total_x - self._layout_params.margin
-                for child, size in zip(right["children"], right["sizes"]):
-                    child.set_position(x_now - size[0], y_cen - size[1] / 2)
-                    x_now -= size[0] + self._layout_params.padding
-
-                    # top
-                y_now = self._layout_params.margin
-                for child, size in zip(top["children"], top["sizes"]):
-                    child.set_position(x_cen - size[0] / 2, y_now)
-                    y_now += size[1] + self._layout_params.padding
-
-                    # bottom
-                y_now = total_y - self._layout_params.margin
-                for child, size in zip(bottom["children"], bottom["sizes"]):
-                    child.set_position(x_cen - size[0] / 2, y_now - size[1])
-                    y_now -= size[1] + self._layout_params.padding
-
-            case Layout.Grid:
-                rows: list[dict[str, tp.Any | float]] = []
-                columns: list[dict[str, tp.Any | float]] = []
-
-                for child, params in self._child_params:
-                    row, column = params["row"], params["column"]
-
-                    # if row was not yet made, make all previous ones
-                    if len(rows) <= row:
-                        for n_row in range(len(rows), row + 1):
-                            out = {
-                                "weight": 0,
-                                "children": []
-                            }
-
-                            if n_row in self._grid_params.rows:
-                                config = self._grid_params.rows[n_row]
-
-                                if "weight" in config:
-                                    out["weight"] = config["weight"]
-
-                            rows.append(out)
-
-                    if len(columns) <= column:
-                        for n_col in range(len(columns), column + 1):
-                            out = {
-                                "weight": 0,
-                                "children": []
-                            }
-
-                            if n_col in self._grid_params.columns:
-                                config = self._grid_params.columns[n_col]
-
-                                if "weight" in config:
-                                    out["weight"] = config["weight"]
-
-                            columns.append(out)
-
-                    rows[row]["children"].append((child, params))
-                    columns[column]["children"].append((child, params))
-
-                matrix: list[list] = []
-
-                for r in range(len(rows)):
-                    matrix.append([])
-
-                    for c in range(len(columns)):
-                        # child = set(rows[r]["children"]) & set(columns[c]["children"])
-                        child = [chi for chi in rows[r]["children"] if chi in columns[c]["children"]]
-                        child = list(child)
-
-                        if len(child) > 1:
-                            raise ValueError(f"{len(child)} children assigned to row {r} column {c}!")
-
-                        if child:
-                            matrix[r].append(child[0])
-
-                        else:
-                            matrix[r].append(...)
-
-                # calculate the minimal size for each row
-                for r, row in enumerate(rows):
-                    rows[r]["max_size"] = 0
-
-                    for child, params in row["children"]:
-                        _, y = child.calculate_size()
-
-                        y += 2 * params.margin
-
-                        if y > rows[r]["max_size"]:
-                            rows[r]["max_size"] = y
-
-                # calculate the minimal size for each column
-                for c, column in enumerate(columns):
-                    columns[c]["max_size"] = 0
-
-                    for child, params in column["children"]:
-                        x, _ = child.calculate_size()
-
-                        x += 2 * params.margin
-
-                        if x > columns[c]["max_size"]:
-                            columns[c]["max_size"] = x
-
-                    # calculate the container size
-                width, height = self.calculate_size()
-
-                # only subtract rows that don't have a weight
-                min_width = sum([c["max_size"] for c in columns])
-                min_height = sum([r["max_size"] for r in rows])
-
-                # set the windows minimal size
-                self._min_size = min_width, min_height
-
-                # assign extra space
-                extra_width = width - sum([c["max_size"] for c in columns if c["weight"] == 0])
-                extra_height = height - sum([r["max_size"] for r in rows if r["weight"] == 0])
-
-                total_row_weight = sum([row["weight"] for row in rows])
-                total_column_weight = sum([column["weight"] for column in columns])
-
-                # print(f"\n\nwindow_size=[{width}, {height}]\tmin_size={[min_width, min_height]}")
-                # print(f"{total_row_weight=}")
-                # print(f"{total_column_weight=}")
-                # print(f"{extra_height=}")
-                # print(f"{extra_width=}")
-
-                # assign each row and column a specific size
-                for r in range(len(rows)):
-                    if total_row_weight == 0:
-                        rows[r]["height"] = 0
-                    else:
-                        # assign either the minimum size or the calculated dynamic one
-                        w_size = ((rows[r]["weight"] / total_row_weight) * extra_height).__floor__()
-                        rows[r]["height"] = max([w_size, rows[r]["max_size"]])
-                        # print(f"{w_size=}\t{rows[r]['max_size']=}")
-
-                    # rows[r]["height"] += rows[r]["max_size"]
-                    rows[r]["y_start"] = sum([prev_row["height"] for prev_row in rows[:r]])
-
-                    for c in range(len(columns)):
-                        if total_column_weight == 0:
-                            columns[c]["width"] = 0
-                        else:
-                            # assign either the minimum size or the calculated dynamic one
-                            w_size = ((columns[c]["weight"] / total_column_weight) * extra_width).__floor__()
-                            columns[c]["width"] = max([w_size, columns[c]["max_size"]])
-                            # print(f"{w_size=}\t{columns[c]['max_size']=}")
-
-                        # columns[c]["width"] += columns[c]["max_size"]
-                        columns[c]["x_start"] = sum([prev_col["width"] for prev_col in columns[:c]])
-
-                        # pg.draw.rect(
-                        #     self.__background,
-                        #     (255, 0, 0, 255),
-                        #     pg.Rect(columns[c]["x_start"], rows[r]["y_start"], columns[c]["width"], rows[r]["height"]),
-                        #     width=1
-                        # )
-
-                # place children
-                for child, params in self._child_params:
-                    # place the child proportional to the table and stickiness
-                    # size = list(child.calculate_size())
-                    size = [child._width, child._height]
-
-                    row, column = params["row"], params["column"]
-                    sticky = params["sticky"]
-
-                    width = columns[column]["width"]
-                    height = rows[row]["height"]
-
-                    x = columns[column]["x_start"]
-                    y = rows[row]["y_start"]
-
-                    x_cen = x + width / 2
-                    y_cen = y + height / 2
-
-                    x_diff = width - size[0]
-                    y_diff = height - size[1]
-
-                    # print(f"calc: {x_diff}, {y_diff}\t{size}\t{width},{height}")
-                    # print(f"{sticky=}")
-
-                    box_x = x_cen - size[0] / 2
-                    box_y = y_cen - size[1] / 2
-
-                    # assign stickiness
-                    if not child._width_configured:
-                        if "w" in sticky:
-                            size[0] += (x_diff / 2) - params.margin
-                            box_x = x + params.margin
-
-                        if "e" in sticky:
-                            size[0] += (x_diff / 2) - params.margin
-
-                        child.assigned_width = size[0]
-
-                    if not child._height_configured:
-                        if "n" in sticky:
-                            size[1] += (y_diff / 2) - params.margin
-                            box_y = y + params.margin
-                            # print("north: ", size, box_x, box_y, "\t\t", width, height)
-
-                        if "s" in sticky:
-                            size[1] += (y_diff / 2) - params.margin
-                            # print("south: ", size, box_x, box_y, "\t\t", width, height)
-
-                        child.assigned_height = size[1]
-
-                    child.set_position(box_x, box_y)
-
-            case _:
-                raise ValueError(f"Invalid geometry type: {self._layout.__class__.__name__}")
+    # def calculate_geometry(self):
+    #     """
+    #     calculate how each individual child should be placed
+    #     """
+    #     match self._layout:
+    #         case Layout.Absolute:  # Absolute
+    #             # since the positioning is absolute, the children should not influence the parents size
+    #             for child, params in self._child_params:
+    #                 child.set_position(params.x, params.y)
+    #
+    #             return
+    #
+    #         case Layout.Pack:
+    #             directional_dict: dict[str, int | list] = {"total_x": 0, "total_y": 0, "children": [], "sizes": []}
+    #             top = deepcopy(directional_dict)
+    #             bottom = deepcopy(directional_dict)
+    #             left = deepcopy(directional_dict)
+    #             right = deepcopy(directional_dict)
+    #
+    #             # get all sizes and group by anchor
+    #             for child, param in self._child_params:
+    #                 child_size = child.calculate_size()
+    #
+    #                 if param.anchor == TOP:
+    #                     top["children"].append(child)
+    #                     top["sizes"].append(child_size)
+    #                     top["total_x"] += child_size[0]
+    #                     top["total_y"] += child_size[1]
+    #
+    #                 elif param.anchor == BOTTOM:
+    #                     bottom["children"].append(child)
+    #                     bottom["sizes"].append(child_size)
+    #                     bottom["total_x"] += child_size[0]
+    #                     bottom["total_y"] += child_size[1]
+    #
+    #                 elif param.anchor == LEFT:
+    #                     left["children"].append(child)
+    #                     left["sizes"].append(child_size)
+    #                     left["total_x"] += child_size[0]
+    #                     left["total_y"] += child_size[1]
+    #
+    #                 elif param.anchor == RIGHT:
+    #                     right["children"].append(child)
+    #                     right["sizes"].append(child_size)
+    #                     right["total_x"] += child_size[0]
+    #                     right["total_y"] += child_size[1]
+    #
+    #             top["total_y"] += self._layout_params.padding * len(top["children"]) - 1
+    #             bottom["total_y"] += self._layout_params.padding * len(bottom["children"]) - 1
+    #
+    #             left["total_x"] += self._layout_params.padding * len(left["children"]) - 1
+    #             right["total_x"] += self._layout_params.padding * len(right["children"]) - 1
+    #
+    #             min_x = max([top["total_x"], bottom["total_x"], left["total_x"] + right["total_x"]])
+    #             min_y = max([left["total_y"], right["total_y"], top["total_y"] + bottom["total_y"]])
+    #
+    #             # add margin
+    #             min_x += self.layout_params.margin * 2
+    #             min_y += self.layout_params.margin * 2
+    #
+    #             self._min_size = min_x, min_y
+    #
+    #             total_x, total_y = self.calculate_size()
+    #
+    #             # tell the children where they should be
+    #             y_cen = total_y / 2
+    #             x_cen = total_x / 2
+    #
+    #             # left
+    #             x_now = self._layout_params.margin
+    #             for child, size in zip(left["children"], left["sizes"]):
+    #                 child.set_position(x_now, y_cen - size[1] / 2)
+    #                 x_now += size[0] + self._layout_params.padding
+    #
+    #                 # right
+    #             x_now = total_x - self._layout_params.margin
+    #             for child, size in zip(right["children"], right["sizes"]):
+    #                 child.set_position(x_now - size[0], y_cen - size[1] / 2)
+    #                 x_now -= size[0] + self._layout_params.padding
+    #
+    #                 # top
+    #             y_now = self._layout_params.margin
+    #             for child, size in zip(top["children"], top["sizes"]):
+    #                 child.set_position(x_cen - size[0] / 2, y_now)
+    #                 y_now += size[1] + self._layout_params.padding
+    #
+    #                 # bottom
+    #             y_now = total_y - self._layout_params.margin
+    #             for child, size in zip(bottom["children"], bottom["sizes"]):
+    #                 child.set_position(x_cen - size[0] / 2, y_now - size[1])
+    #                 y_now -= size[1] + self._layout_params.padding
+    #
+    #         case Layout.Grid:
+    #             rows: list[dict[str, tp.Any | float]] = []
+    #             columns: list[dict[str, tp.Any | float]] = []
+    #
+    #             for child, params in self._child_params:
+    #                 row, column = params["row"], params["column"]
+    #
+    #                 # if row was not yet made, make all previous ones
+    #                 if len(rows) <= row:
+    #                     for n_row in range(len(rows), row + 1):
+    #                         out = {
+    #                             "weight": 0,
+    #                             "children": []
+    #                         }
+    #
+    #                         if n_row in self._grid_params.rows:
+    #                             config = self._grid_params.rows[n_row]
+    #
+    #                             if "weight" in config:
+    #                                 out["weight"] = config["weight"]
+    #
+    #                         rows.append(out)
+    #
+    #                 if len(columns) <= column:
+    #                     for n_col in range(len(columns), column + 1):
+    #                         out = {
+    #                             "weight": 0,
+    #                             "children": []
+    #                         }
+    #
+    #                         if n_col in self._grid_params.columns:
+    #                             config = self._grid_params.columns[n_col]
+    #
+    #                             if "weight" in config:
+    #                                 out["weight"] = config["weight"]
+    #
+    #                         columns.append(out)
+    #
+    #                 rows[row]["children"].append((child, params))
+    #                 columns[column]["children"].append((child, params))
+    #
+    #             matrix: list[list] = []
+    #
+    #             for r in range(len(rows)):
+    #                 matrix.append([])
+    #
+    #                 for c in range(len(columns)):
+    #                     # child = set(rows[r]["children"]) & set(columns[c]["children"])
+    #                     child = [chi for chi in rows[r]["children"] if chi in columns[c]["children"]]
+    #                     child = list(child)
+    #
+    #                     if len(child) > 1:
+    #                         raise ValueError(f"{len(child)} children assigned to row {r} column {c}!")
+    #
+    #                     if child:
+    #                         matrix[r].append(child[0])
+    #
+    #                     else:
+    #                         matrix[r].append(...)
+    #
+    #             # calculate the minimal size for each row
+    #             for r, row in enumerate(rows):
+    #                 rows[r]["max_size"] = 0
+    #
+    #                 for child, params in row["children"]:
+    #                     _, y = child.calculate_size()
+    #
+    #                     y += 2 * params.margin
+    #
+    #                     if y > rows[r]["max_size"]:
+    #                         rows[r]["max_size"] = y
+    #
+    #             # calculate the minimal size for each column
+    #             for c, column in enumerate(columns):
+    #                 columns[c]["max_size"] = 0
+    #
+    #                 for child, params in column["children"]:
+    #                     x, _ = child.calculate_size()
+    #
+    #                     x += 2 * params.margin
+    #
+    #                     if x > columns[c]["max_size"]:
+    #                         columns[c]["max_size"] = x
+    #
+    #                 # calculate the container size
+    #             width, height = self.calculate_size()
+    #
+    #             # only subtract rows that don't have a weight
+    #             min_width = sum([c["max_size"] for c in columns])
+    #             min_height = sum([r["max_size"] for r in rows])
+    #
+    #             # set the windows minimal size
+    #             self._min_size = min_width, min_height
+    #
+    #             # assign extra space
+    #             extra_width = width - sum([c["max_size"] for c in columns if c["weight"] == 0])
+    #             extra_height = height - sum([r["max_size"] for r in rows if r["weight"] == 0])
+    #
+    #             total_row_weight = sum([row["weight"] for row in rows])
+    #             total_column_weight = sum([column["weight"] for column in columns])
+    #
+    #             # print(f"\n\nwindow_size=[{width}, {height}]\tmin_size={[min_width, min_height]}")
+    #             # print(f"{total_row_weight=}")
+    #             # print(f"{total_column_weight=}")
+    #             # print(f"{extra_height=}")
+    #             # print(f"{extra_width=}")
+    #
+    #             # assign each row and column a specific size
+    #             for r in range(len(rows)):
+    #                 if total_row_weight == 0:
+    #                     rows[r]["height"] = 0
+    #                 else:
+    #                     # assign either the minimum size or the calculated dynamic one
+    #                     w_size = ((rows[r]["weight"] / total_row_weight) * extra_height).__floor__()
+    #                     rows[r]["height"] = max([w_size, rows[r]["max_size"]])
+    #                     # print(f"{w_size=}\t{rows[r]['max_size']=}")
+    #
+    #                 # rows[r]["height"] += rows[r]["max_size"]
+    #                 rows[r]["y_start"] = sum([prev_row["height"] for prev_row in rows[:r]])
+    #
+    #                 for c in range(len(columns)):
+    #                     if total_column_weight == 0:
+    #                         columns[c]["width"] = 0
+    #                     else:
+    #                         # assign either the minimum size or the calculated dynamic one
+    #                         w_size = ((columns[c]["weight"] / total_column_weight) * extra_width).__floor__()
+    #                         columns[c]["width"] = max([w_size, columns[c]["max_size"]])
+    #                         # print(f"{w_size=}\t{columns[c]['max_size']=}")
+    #
+    #                     # columns[c]["width"] += columns[c]["max_size"]
+    #                     columns[c]["x_start"] = sum([prev_col["width"] for prev_col in columns[:c]])
+    #
+    #                     # pg.draw.rect(
+    #                     #     self.__background,
+    #                     #     (255, 0, 0, 255),
+    #                     #     pg.Rect(columns[c]["x_start"], rows[r]["y_start"], columns[c]["width"], rows[r]["height"]),
+    #                     #     width=1
+    #                     # )
+    #
+    #             # place children
+    #             for child, params in self._child_params:
+    #                 # place the child proportional to the table and stickiness
+    #                 # size = list(child.calculate_size())
+    #                 size = [child._width, child._height]
+    #
+    #                 row, column = params["row"], params["column"]
+    #                 sticky = params["sticky"]
+    #
+    #                 width = columns[column]["width"]
+    #                 height = rows[row]["height"]
+    #
+    #                 x = columns[column]["x_start"]
+    #                 y = rows[row]["y_start"]
+    #
+    #                 x_cen = x + width / 2
+    #                 y_cen = y + height / 2
+    #
+    #                 x_diff = width - size[0]
+    #                 y_diff = height - size[1]
+    #
+    #                 # print(f"calc: {x_diff}, {y_diff}\t{size}\t{width},{height}")
+    #                 # print(f"{sticky=}")
+    #
+    #                 box_x = x_cen - size[0] / 2
+    #                 box_y = y_cen - size[1] / 2
+    #
+    #                 # assign stickiness
+    #                 if not child._width_configured:
+    #                     if "w" in sticky:
+    #                         size[0] += (x_diff / 2) - params.margin
+    #                         box_x = x + params.margin
+    #
+    #                     if "e" in sticky:
+    #                         size[0] += (x_diff / 2) - params.margin
+    #
+    #                     child.assigned_width = size[0]
+    #
+    #                 if not child._height_configured:
+    #                     if "n" in sticky:
+    #                         size[1] += (y_diff / 2) - params.margin
+    #                         box_y = y + params.margin
+    #                         # print("north: ", size, box_x, box_y, "\t\t", width, height)
+    #
+    #                     if "s" in sticky:
+    #                         size[1] += (y_diff / 2) - params.margin
+    #                         # print("south: ", size, box_x, box_y, "\t\t", width, height)
+    #
+    #                     child.assigned_height = size[1]
+    #
+    #                 child.set_position(box_x, box_y)
+    #
+    #         case _:
+    #             raise ValueError(f"Invalid geometry type: {self._layout.__class__.__name__}")
 
     def calculate_size(self) -> tuple[int, int]:
         """
         calculate how big the container should be
         """
         # make sure the geometry is up-to-date
         return pg.display.get_window_size()
```

### Comparing `pginter-0.2.3/src/pginter/icon.png` & `pginter-0.2.4/src/pginter/icon.png`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/theme/_manager.py` & `pginter-0.2.4/src/pginter/theme/_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/theme/themes/default.json` & `pginter-0.2.4/src/pginter/theme/themes/default.json`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/types/_color.py` & `pginter-0.2.4/src/pginter/types/_color.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/types/_scheme.py` & `pginter-0.2.4/src/pginter/types/_scheme.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/types/_style.py` & `pginter-0.2.4/src/pginter/types/_style.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/types/_tk_vars.py` & `pginter-0.2.4/src/pginter/types/_tk_vars.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/utils/_funcs.py` & `pginter-0.2.4/src/pginter/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_button.py` & `pginter-0.2.4/src/pginter/widgets/_button.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_entry.py` & `pginter-0.2.4/src/pginter/widgets/_entry.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_frame.py` & `pginter-0.2.4/src/pginter/widgets/_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_geo_manager.py` & `pginter-0.2.4/src/pginter/widgets/_geo_manager.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_label.py` & `pginter-0.2.4/src/pginter/widgets/_label.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter/widgets/_surface_frame.py` & `pginter-0.2.4/src/pginter/widgets/_surface_frame.py`

 * *Files identical despite different names*

### Comparing `pginter-0.2.3/src/pginter.egg-info/SOURCES.txt` & `pginter-0.2.4/src/pginter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

