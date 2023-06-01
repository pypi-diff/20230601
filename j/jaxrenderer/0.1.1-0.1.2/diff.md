# Comparing `tmp/jaxrenderer-0.1.1.tar.gz` & `tmp/jaxrenderer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.1.1.tar", max compression
+gzip compressed data, was "jaxrenderer-0.1.2.tar", max compression
```

## Comparing `jaxrenderer-0.1.1.tar` & `jaxrenderer-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11367 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/LICENSE
--rw-r--r--   0        0        0     1700 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/README.md
--rw-r--r--   0        0        0     3019 2023-05-31 09:43:25.069668 jaxrenderer-0.1.1/changelog.md
--rw-r--r--   0        0        0     1541 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/README.md
--rw-r--r--   0        0        0      459 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/__init__.py
--rw-r--r--   0        0        0    33807 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/geometry.py
--rw-r--r--   0        0        0    14829 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/model.py
--rw-r--r--   0        0        0    11913 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/pipeline.py
--rw-r--r--   0        0        0    13303 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/renderer.py
--rw-r--r--   0        0        0     9726 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/types.py
--rw-r--r--   0        0        0     3074 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-05-31 09:43:25.073668 jaxrenderer-0.1.1/renderer/value_checker.py
--rw-r--r--   0        0        0     3105 1970-01-01 00:00:00.000000 jaxrenderer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-01 15:40:54.196204 jaxrenderer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1700 2023-06-01 15:40:54.196204 jaxrenderer-0.1.2/README.md
+-rw-r--r--   0        0        0     3758 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/changelog.md
+-rw-r--r--   0        0        0     1540 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/README.md
+-rw-r--r--   0        0        0      459 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/__init__.py
+-rw-r--r--   0        0        0    33682 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/geometry.py
+-rw-r--r--   0        0        0    14815 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/model.py
+-rw-r--r--   0        0        0    11913 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/pipeline.py
+-rw-r--r--   0        0        0    13485 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/renderer.py
+-rw-r--r--   0        0        0     9726 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/types.py
+-rw-r--r--   0        0        0     3074 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/value_checker.py
+-rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 jaxrenderer-0.1.2/PKG-INFO
```

### Comparing `jaxrenderer-0.1.1/LICENSE` & `jaxrenderer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/README.md` & `jaxrenderer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/changelog.md` & `jaxrenderer-0.1.2/changelog.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,7 +21,15 @@
 5. `Scene.set_object_orientation` and `Scene.set_object_local_scaling` supports tuple of floats as well as inputs, additional to `jnp.array`.
 6. `Model` now has a convenient method `create` to create a Model with same face indices shared by `faces`, `faces_norm` and `faces_uv`, and a default `specular_map`. This is useful for creating a mesh where all vertices has its own normal and uv coordinate specified, under same order (thus same face indices).
 7. Correctly support Python Sequence for `utils.build_texture_from_PyTinyrenderer` as texture.
 8. `quaternion` function to create an orientation from axis and angle, and `quaternion_mul` to composite quaternion.
 9. `rotation_matrix` function to create a rotation matrix from axis and angle. Also allows `Scene` to set object orientation directly using rotation matrix.
 10. Move `Renderer.merge_objects` into `geometry.py`, and expose in `__init__.py`.
 11. `batch_models` and `Renderer.create_buffers` convenient method to facilitate batch rendering of multiple models.
+
+## 0.1.2
+
+1. Change the ordering of quaternions (in `geometry.py`) to `(w, x, y, z)` instead of `(x, y, z, w)` to be consistent with the convention used in `pytinyrenderer` and `BRAX`. Reference: [brax/math.py](https://github.com/google/brax/blob/aebd8b8cb34430f6eaf6f914293f901e3c8d9a22/brax/math.py).
+2. Fix: remove unnecessary `@staticmethod` decorator in `merge_objects`.
+3. Changed the way that `Camera` is created in `Renderer.create_camera_from_parameters` to force convert parameters into `float` weak type.
+4. Force convert `LightParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
+5. Downgrade minimum Python version to `3.9`, `numpy` version to `1.22.0`, `jax` and `jaxlib` version to `0.4.4`.
```

### Comparing `jaxrenderer-0.1.1/pyproject.toml` & `jaxrenderer-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.1.1"
+version = "0.1.2"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
@@ -28,18 +28,18 @@
     "README.md",
     "changelog.md",
     "pyproject.toml",
 ]
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
-jax = "^0.4.8"
-numpy = "^1.24.1"
-jaxlib = {version = "^0.4.7", source = "jax"}
+python = "^3.9"
+jax = "^0.4.4"
+numpy = "^1.22.0"
+jaxlib = {version = "^0.4.4", source = "jax"}
 jaxtyping = "^0.2.19"
 importlib-metadata = "^6.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.6.2"
 pillow = "^9.4.0"
```

### Comparing `jaxrenderer-0.1.1/renderer/README.md` & `jaxrenderer-0.1.2/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/geometry.py` & `jaxrenderer-0.1.2/renderer/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -828,59 +828,56 @@
     rotation_axis: Union[Vec3f, tuple[float, float, float]],
     rotation_angle: Union[Float[Array, ""], float],
 ) -> Vec4f:
     """Generate a quaternion rotation from a rotation axis and angle.
 
     The rotation axis is normalised internally. The angle is specified in
     degrees (NOT radian). The rotation is clockwise.
+
+    The resultant quaternion is in order of (w, x, y, z).
     """
     axis = normalise(jnp.asarray(rotation_axis))
     angle = jnp.radians(jnp.asarray(rotation_angle))
     assert isinstance(axis, Vec3f), f"{rotation_axis}"
     assert isinstance(angle, Float[Array, ""]), f"{rotation_angle}"
 
     quaternion: Vec4f = (
         jnp.zeros(4)  #
-        .at[:3].set(axis * jnp.sin(angle / 2))  #
-        .at[3].set(jnp.cos(angle / 2))  #
+        .at[0].set(jnp.cos(angle / 2))  #
+        .at[1:].set(axis * jnp.sin(angle / 2))  #
     )
 
     return quaternion
 
 
 @jaxtyped
 @jax.jit
 def quaternion_mul(quatA: Vec4f, quatB: Vec4f) -> Vec4f:
     """Multiply two quaternion rotations, as to composite them.
 
-    Noticed that all quaternions here are in order of (x, y, z, w), thus
-    shuffles are used here to convert from (w, x, y, z) to (x, y, z, w).
+    Noticed that all quaternions here are in order of (w, x, y, z).
 
     References:
       - [Quaternion multiplication](https://www.mathworks.com/help/nav/ref/quaternion.mtimes.html)
     """
     assert isinstance(quatA, Vec4f)
     assert isinstance(quatB, Vec4f)
 
     with jax.ensure_compile_time_eval():
-        shuffle = jnp.array((3, 0, 1, 2))
         idx103 = jnp.array((1, 0, 3))
         idx230 = jnp.array((2, 3, 0))
         idx013 = jnp.array((0, 1, 3))
         idx320 = jnp.array((3, 2, 0))
 
-    quatA = quatA[shuffle]
-    quatB = quatB[shuffle]
-
     return jnp.array((
         quatA[0] * quatB[0] - quatA[1:] @ quatB[1:],
         quatA[:3] @ quatB[idx103] - quatA[3] * quatB[2],
         quatA[idx230] @ quatB[:3] - quatA[1] * quatB[3],
         quatA[idx013] @ quatB[idx320] - quatA[2] * quatB[1],
-    ))[shuffle]
+    ))
 
 
 @jaxtyped
 @jax.jit
 def rotation_matrix(
     rotation_axis: Union[Vec3f, tuple[float, float, float]],
     rotation_angle: Union[Float[Array, ""], float],
```

### Comparing `jaxrenderer-0.1.1/renderer/model.py` & `jaxrenderer-0.1.2/renderer/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,14 @@
         [jnp.asarray(model[i])[None, ...] for model in models],
         dimension=0,
     ) for i in range(len(models[0]))))
 
     return merged_model
 
 
-@staticmethod
 @jaxtyped
 def merge_objects(objects: Sequence[ModelObject]) -> MergedModel:
     """Merge objects into a single model.
 
     Parameters:
       - objects: a list of objects to merge.
```

### Comparing `jaxrenderer-0.1.1/renderer/pipeline.py` & `jaxrenderer-0.1.2/renderer/pipeline.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/renderer.py` & `jaxrenderer-0.1.2/renderer/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from functools import partial
 from typing import NamedTuple, Optional, Sequence, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
+from jax.tree_util import tree_map
 from jaxtyping import Array, Bool, Integer, Num, jaxtyped
 
 from .geometry import Camera, Projection, View, Viewport, normalise
 from .model import MergedModel, ModelObject, merge_objects
 from .pipeline import render
 from .shaders.phong_reflection import (PhongReflectionTextureExtraInput,
                                        PhongReflectionTextureShader)
@@ -97,19 +98,19 @@
 class Renderer:
 
     @staticmethod
     @jaxtyped
     @partial(jax.jit, inline=True)
     def create_camera_from_parameters(camera: CameraParameters) -> Camera:
         """Create a camera from camera parameters."""
-        eye: Vec3f = jnp.asarray(camera.position)
+        eye: Vec3f = jnp.asarray(camera.position, dtype=float)
         assert isinstance(eye, Vec3f), f"{eye}"
-        centre: Vec3f = jnp.asarray(camera.target)
+        centre: Vec3f = jnp.asarray(camera.target, dtype=float)
         assert isinstance(centre, Vec3f), f"{centre}"
-        up: Vec3f = jnp.asarray(camera.up)
+        up: Vec3f = jnp.asarray(camera.up, dtype=float)
         assert isinstance(up, Vec3f), f"{up}"
 
         view_mat: View = Camera.view_matrix(eye=eye, centre=centre, up=up)
         assert isinstance(view_mat, View), f"{view_mat}"
         view_inv: View = Camera.view_matrix_inv(eye=eye, centre=centre, up=up)
         assert isinstance(view_inv, View), f"{view_inv}"
         projection_mat: Projection = Camera.perspective_projection_matrix(
@@ -325,14 +326,17 @@
         if isinstance(camera, CameraParameters):
             _camera = cls.create_camera_from_parameters(camera)
         else:
             _camera = camera
 
         assert isinstance(_camera, Camera), f"{_camera}"
 
+        light = tree_map(jnp.asarray, light)
+        assert isinstance(light, LightParameters), f"{light}"
+
         buffers: Buffers = cls.create_buffers(
             width=width,
             height=height,
             colour_default=colour_default,
             zbuffer_default=zbuffer_default,
         )
```

### Comparing `jaxrenderer-0.1.1/renderer/scene.py` & `jaxrenderer-0.1.2/renderer/scene.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shader.py` & `jaxrenderer-0.1.2/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/README.md` & `jaxrenderer-0.1.2/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/depth.py` & `jaxrenderer-0.1.2/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/gouraud.py` & `jaxrenderer-0.1.2/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.1.2/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/phong.py` & `jaxrenderer-0.1.2/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.1.2/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.1.2/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.1.2/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shadow.py` & `jaxrenderer-0.1.2/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shapes/capsule.py` & `jaxrenderer-0.1.2/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/shapes/cube.py` & `jaxrenderer-0.1.2/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/types.py` & `jaxrenderer-0.1.2/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/utils.py` & `jaxrenderer-0.1.2/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/renderer/value_checker.py` & `jaxrenderer-0.1.2/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.1/PKG-INFO` & `jaxrenderer-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Graphics :: 3D Rendering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Typing :: Typed
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
-Requires-Dist: jax (>=0.4.8,<0.5.0)
-Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
+Requires-Dist: jax (>=0.4.4,<0.5.0)
+Requires-Dist: jaxlib (>=0.4.4,<0.5.0)
 Requires-Dist: jaxtyping (>=0.2.19,<0.3.0)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/JoeyTeng/jaxrenderer/issues
 Project-URL: Repository, https://github.com/JoeyTeng/jaxrenderer
 Description-Content-Type: text/markdown
 
 # JAX Renderer
 
 ## Key Difference from [erwincoumans/tinyrenderer](https://github.com/erwincoumans/tinyrenderer)
```

