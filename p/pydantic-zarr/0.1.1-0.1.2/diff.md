# Comparing `tmp/pydantic_zarr-0.1.1.tar.gz` & `tmp/pydantic_zarr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.1.1.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.1.2.tar", max compression
```

## Comparing `pydantic_zarr-0.1.1.tar` & `pydantic_zarr-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.1/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.1/README.md
--rw-r--r--   0        0        0      489 2023-06-01 18:49:19.092277 pydantic_zarr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 17:37:02.193613 pydantic_zarr-0.1.1/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0     7743 2023-06-01 18:39:09.877146 pydantic_zarr-0.1.1/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.2/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.2/README.md
+-rw-r--r--   0        0        0      489 2023-06-01 19:07:18.430532 pydantic_zarr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 17:37:02.193613 pydantic_zarr-0.1.2/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0     8330 2023-06-01 19:05:25.338950 pydantic_zarr-0.1.2/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.2/PKG-INFO
```

### Comparing `pydantic_zarr-0.1.1/LICENSE` & `pydantic_zarr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.1.1/src/pydantic_zarr/core.py` & `pydantic_zarr-0.1.2/src/pydantic_zarr/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,27 +68,30 @@
 
         """
 
         filters = zarray.filters
         if filters is not None:
             filters = [f.get_config() for f in filters]
 
+        compressor = zarray.compressor
+        if compressor is not None:
+            compressor = compressor.get_config()
         return cls(
             shape=zarray.shape,
             chunks=zarray.chunks,
             dtype=str(zarray.dtype),
             fill_value=zarray.fill_value,
             order=zarray.order,
             filters=filters,
             dimension_separator=zarray._dimension_separator,
-            compressor=zarray.compressor.get_config(),
+            compressor=compressor,
             attrs=dict(zarray.attrs),
         )
 
-    def to_zarr(self, store, path) -> zarr.Array:
+    def to_zarr(self, store: BaseStore, path: str) -> zarr.Array:
         """
         Serialize an ArraySpec to a zarr array at a specific path in a zarr store.
 
         Parameters
         ----------
         store : instance of zarr.BaseStore
             The storage backend that will manifest the array.
@@ -99,16 +102,17 @@
         Returns
         -------
         A zarr array that is structurally identical to the ArraySpec.
         This operation will create metadata documents in the store.
         """
         spec_dict = self.dict()
         attrs = spec_dict.pop("attrs")
-        spec_dict["compressor"] = numcodecs.get_codec(spec_dict["compressor"])
-        if spec_dict["filters"] is not None:
+        if self.compressor is not None:
+            spec_dict["compressor"] = numcodecs.get_codec(spec_dict["compressor"])
+        if self.filters is not None:
             spec_dict["filters"] = [
                 numcodecs.get_codec(f) for f in spec_dict["filters"]
             ]
         result = zarr.create(store=store, path=path, **spec_dict)
         result.attrs.put(attrs)
         return result
 
@@ -136,14 +140,20 @@
         result: GroupSpec
         items = {}
         for name, item in zgroup.items():
             if isinstance(item, zarr.Array):
                 _item = ArraySpec.from_zarr(item)
             elif isinstance(item, zarr.Group):
                 _item = cls.from_zarr(item)
+            else:
+                msg = f"""
+                Unparseable object encountered: {type(item)}. Expected zarr.Array or
+                zarr.Group.
+                """
+                raise ValueError(msg)
             items[name] = _item
 
         result = GroupSpec(attrs=dict(zgroup.attrs), items=items)
         return result
 
     def to_zarr(self, store: BaseStore, path: str):
         """
@@ -196,14 +206,20 @@
     elif isinstance(element, zarr.Group):
         items = {}
         for name, item in element.items():
             if isinstance(item, zarr.Array):
                 _item = ArraySpec.from_zarr(item)
             elif isinstance(item, zarr.Group):
                 _item = GroupSpec.from_zarr(item)
+            else:
+                msg = f"""
+                Unparseable object encountered: {type(item)}. Expected zarr.Array or
+                zarr.Group.
+                """
+                raise ValueError(msg)
             items[name] = _item
 
         result = GroupSpec(attrs=dict(element.attrs), items=items)
         return result
     else:
         msg = f"""
         Object of type {type(element)} cannot be processed by this function.
```

### Comparing `pydantic_zarr-0.1.1/PKG-INFO` & `pydantic_zarr-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-zarr
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

