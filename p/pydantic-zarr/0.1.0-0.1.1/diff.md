# Comparing `tmp/pydantic_zarr-0.1.0.tar.gz` & `tmp/pydantic_zarr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_zarr-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_zarr-0.1.1.tar", max compression
```

## Comparing `pydantic_zarr-0.1.0.tar` & `pydantic_zarr-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.0/LICENSE
--rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.0/README.md
--rw-r--r--   0        0        0      490 2023-06-01 14:41:34.156488 pydantic_zarr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 17:37:02.193613 pydantic_zarr-0.1.0/src/pydantic_zarr/__init__.py
--rw-r--r--   0        0        0     7482 2023-06-01 15:39:38.393496 pydantic_zarr-0.1.0/src/pydantic_zarr/core.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-30 21:01:34.647934 pydantic_zarr-0.1.1/LICENSE
+-rw-r--r--   0        0        0      505 2023-05-31 17:55:46.852124 pydantic_zarr-0.1.1/README.md
+-rw-r--r--   0        0        0      489 2023-06-01 18:49:19.092277 pydantic_zarr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 17:37:02.193613 pydantic_zarr-0.1.1/src/pydantic_zarr/__init__.py
+-rw-r--r--   0        0        0     7743 2023-06-01 18:39:09.877146 pydantic_zarr-0.1.1/src/pydantic_zarr/core.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pydantic_zarr-0.1.1/PKG-INFO
```

### Comparing `pydantic_zarr-0.1.0/LICENSE` & `pydantic_zarr-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_zarr-0.1.0/src/pydantic_zarr/core.py` & `pydantic_zarr-0.1.1/src/pydantic_zarr/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Optional,
     TypeVar,
     Union,
 )
 
 from pydantic.generics import GenericModel
 from zarr.storage import init_group, BaseStore
+import numcodecs
 import zarr
 import os
 
 TAttrs = TypeVar("TAttrs", bound=dict[str, Any])
 TItem = TypeVar("TItem", bound=Union["ArraySpec", "GroupSpec"])
 
 DimensionSeparator = Union[Literal["."], Literal["/"]]
@@ -98,14 +99,19 @@
         Returns
         -------
         A zarr array that is structurally identical to the ArraySpec.
         This operation will create metadata documents in the store.
         """
         spec_dict = self.dict()
         attrs = spec_dict.pop("attrs")
+        spec_dict["compressor"] = numcodecs.get_codec(spec_dict["compressor"])
+        if spec_dict["filters"] is not None:
+            spec_dict["filters"] = [
+                numcodecs.get_codec(f) for f in spec_dict["filters"]
+            ]
         result = zarr.create(store=store, path=path, **spec_dict)
         result.attrs.put(attrs)
         return result
 
 
 class GroupSpec(NodeSpec, Generic[TAttrs, TItem]):
     items: dict[str, TItem] = {}
@@ -167,15 +173,15 @@
         result.attrs.put(attrs)
         for name, item in self.items.items():
             subpath = os.path.join(path, name)
             item.to_zarr(store, subpath)
         return result
 
 
-def to_spec(element: Union[zarr.Array, zarr.Group]) -> Union[ArraySpec, GroupSpec]:
+def from_zarr(element: Union[zarr.Array, zarr.Group]) -> Union[ArraySpec, GroupSpec]:
     """
     Recursively parse a Zarr group or Zarr array into an ArraySpec or GroupSpec.
 
     Paramters
     ---------
     element : a zarr Array or zarr Group
 
@@ -204,15 +210,15 @@
         This function can only parse objects that comply with the ArrayLike or 
         GroupLike protocols.
         """
         raise ValueError(msg)
     return result
 
 
-def from_spec(
+def to_zarr(
     spec: Union[ArraySpec, GroupSpec], store: BaseStore, path: str
 ) -> Union[zarr.Array, zarr.Group]:
     """
     Serialize a GroupSpec or ArraySpec to a zarr group or array at a specific path in
     a zarr store.
 
     Parameters
```

### Comparing `pydantic_zarr-0.1.0/PKG-INFO` & `pydantic_zarr-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pydantic-zarr
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: zarr (>=2.14.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pydantic-zarr
```

