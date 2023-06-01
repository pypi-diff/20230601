# Comparing `tmp/bipl-0.1.2.tar.gz` & `tmp/bipl-0.2.0.tar.gz`

## Comparing `bipl-0.1.2.tar` & `bipl-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/py.typed
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_dzi.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_libs.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_openslide.py
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_slide_bases.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/io/_tiff.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/__init__.py
--rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_mosaic.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.1.2/src/bipl/ops/_util.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.1.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.1.2/LICENSE
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.1.2/README.md
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.1.2/hatch_build.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/py.typed
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_dzi.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_libs.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_openslide.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_slide.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_slide_bases.py
+-rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/io/_tiff.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/ops/__init__.py
+-rw-r--r--   0        0        0    14324 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/ops/_mosaic.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 bipl-0.2.0/src/bipl/ops/_util.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 bipl-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bipl-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bipl-0.2.0/README.md
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 bipl-0.2.0/hatch_build.py
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 bipl-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 bipl-0.2.0/PKG-INFO
```

### Comparing `bipl-0.1.2/src/bipl/io/__init__.py` & `bipl-0.2.0/src/bipl/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_dzi.py` & `bipl-0.2.0/src/bipl/io/_dzi.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_libs.py` & `bipl-0.2.0/src/bipl/io/_libs.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_openslide.py` & `bipl-0.2.0/src/bipl/io/_openslide.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/io/_slide.py` & `bipl-0.2.0/src/bipl/io/_slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,21 +107,20 @@
         return f'{type(self).__name__}({line})'
 
     def best_lod_for(self, pool: float) -> tuple[int, Lod]:
         """Gives the most detailed LOD below `pool`"""
         idx = max(bisect_right(self.pools, pool) - 1, 0)
         return self.pools[idx], self.lods[idx]
 
-    def pool(self, zoom: int) -> Lod:
+    def pool(self, zoom: float) -> Lod:
         """Use like `slide.pool(4)[y0:y1, x0:x1]` call"""
-        p, lod = self.best_lod_for(zoom)
+        p, lod = self.best_lod_for(zoom * 1.05)
         if p == zoom:
             return lod
-        assert zoom % p == 0, 'fractional pooling is not supported'
-        return lod.downscale(zoom // p)
+        return lod.rescale(p / zoom)
 
     def __getitem__(self, key: slice | tuple[slice, ...]) -> np.ndarray:
         """Retrieves tile"""
         # TODO: Ignore step, always redirect to self.lods[0].__getitem__
         slices = normalize(key, self.shape)
 
         step0, step1 = (s.step for s in slices)
```

### Comparing `bipl-0.1.2/src/bipl/io/_slide_bases.py` & `bipl-0.2.0/src/bipl/io/_slide_bases.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,34 +58,38 @@
         return self.crop(slices)
 
     @final
     def __array__(self) -> np.ndarray:
         """Reads whole LOD in single call"""
         return self[:, :]
 
-    def downscale(self, pool: int) -> Lod:
-        if pool == 1:
+    def rescale(self, scale: float) -> Lod:
+        if scale == 1:
             return self
         h, w, c = self.shape
         return ProxyLod(
-            (h // pool, w // pool, c),
-            (self.spacing * pool if self.spacing else None),
-            pool,
+            # TODO: round/ceil/floor ?
+            (round(h * scale), round(w * scale), c),
+            (self.spacing / scale if self.spacing else None),
+            scale,
             self.base if isinstance(self, ProxyLod) else self,
         )
 
 
 @dataclass(frozen=True)
 class ProxyLod(Lod):
-    pool: int
+    scale: float
     base: Lod
 
     def crop(self, slices: tuple[slice, ...]) -> np.ndarray:
-        src_slices = *(slice(s.start * self.pool, s.stop * self.pool)
-                       for s in slices),
+        src_slices = *[
+            # TODO: round/ceil/floor ?
+            slice(round(s.start / self.scale), round(s.stop / self.scale))
+            for s in slices
+        ],
         image = self.base[src_slices]
 
         shape = *((s.stop - s.start) for s in slices),
         return cv2.resize(image, shape[::-1], interpolation=cv2.INTER_AREA)
 
 
 class Driver:
```

### Comparing `bipl-0.1.2/src/bipl/io/_tiff.py` & `bipl-0.2.0/src/bipl/io/_tiff.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/ops/_mosaic.py` & `bipl-0.2.0/src/bipl/ops/_mosaic.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/src/bipl/ops/_util.py` & `bipl-0.2.0/src/bipl/ops/_util.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/LICENSE` & `bipl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/README.md` & `bipl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/hatch_build.py` & `bipl-0.2.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bipl-0.1.2/pyproject.toml` & `bipl-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch.build.targets.wheel]
 artifacts = ["*.dll"]  # only wheel keeps DLLs
 
 [tool.hatch.build.hooks.custom]  # enable "custom" hook
 
 [project]
 name = "bipl"
-version = "0.1.2"
+version = "0.2.0"
 description = "Big Image Python Library"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["TIFF", "SVS", "OpenSlide", "tiles"]
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `bipl-0.1.2/PKG-INFO` & `bipl-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipl
-Version: 0.1.2
+Version: 0.2.0
 Summary: Big Image Python Library
 Project-URL: homepage, https://github.com/arquolo/bipl
 Project-URL: repository, https://github.com
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
```

