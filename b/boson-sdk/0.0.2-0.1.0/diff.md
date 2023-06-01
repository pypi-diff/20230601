# Comparing `tmp/boson_sdk-0.0.2-py3-none-any.whl.zip` & `tmp/boson_sdk-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 21179 bytes, number of entries: 15
--rw-r--r--  2.0 unx     1231 b- defN 22-Nov-29 00:15 boson/__init__.py
--rw-r--r--  2.0 unx     3518 b- defN 22-Nov-29 00:15 boson/base.py
--rw-r--r--  2.0 unx     7430 b- defN 22-Nov-29 00:15 boson/boson_v1_pb2.py
--rw-r--r--  2.0 unx     3652 b- defN 22-Nov-29 00:15 boson/conversion.py
--rw-r--r--  2.0 unx     8528 b- defN 22-Nov-29 00:15 boson/features_pb2.py
--rw-r--r--  2.0 unx       57 b- defN 22-Nov-29 00:15 boson/grpc/__init__.py
--rw-r--r--  2.0 unx    13436 b- defN 22-Nov-29 00:15 boson/grpc/boson_v1_pb2_grpc.py
--rw-r--r--  2.0 unx     3160 b- defN 22-Nov-29 00:15 boson/grpc/server.py
--rw-r--r--  2.0 unx       57 b- defN 22-Nov-29 00:15 boson/http/__init__.py
--rw-r--r--  2.0 unx     3898 b- defN 22-Nov-29 00:15 boson/http/server.py
--rw-r--r--  2.0 unx    11356 b- defN 22-Nov-29 00:15 boson_sdk-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    14911 b- defN 22-Nov-29 00:15 boson_sdk-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-29 00:15 boson_sdk-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 22-Nov-29 00:15 boson_sdk-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1170 b- defN 22-Nov-29 00:15 boson_sdk-0.0.2.dist-info/RECORD
-15 files, 72502 bytes uncompressed, 19267 bytes compressed:  73.4%
+Zip file size: 20274 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      749 b- defN 23-Jun-01 20:32 boson/__init__.py
+-rw-r--r--  2.0 unx     3157 b- defN 23-Jun-01 20:32 boson/base.py
+-rw-r--r--  2.0 unx     5320 b- defN 23-Jun-01 20:32 boson/boson_v1_pb2.py
+-rw-r--r--  2.0 unx     3714 b- defN 23-Jun-01 20:32 boson/conversion.py
+-rw-r--r--  2.0 unx     8496 b- defN 23-Jun-01 20:32 boson/features_pb2.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-01 20:32 boson/grpc/__init__.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jun-01 20:32 boson/grpc/boson_v1_pb2_grpc.py
+-rw-r--r--  2.0 unx     2159 b- defN 23-Jun-01 20:32 boson/grpc/server.py
+-rw-r--r--  2.0 unx       57 b- defN 23-Jun-01 20:32 boson/http/__init__.py
+-rw-r--r--  2.0 unx     2568 b- defN 23-Jun-01 20:32 boson/http/server.py
+-rw-r--r--  2.0 unx    11356 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14911 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1168 b- defN 23-Jun-01 20:33 boson_sdk-0.1.0.dist-info/RECORD
+15 files, 59328 bytes uncompressed, 18362 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: boson/http/__init__.py
 Comment: 
 
 Filename: boson/http/server.py
 Comment: 
 
-Filename: boson_sdk-0.0.2.dist-info/LICENSE
+Filename: boson_sdk-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: boson_sdk-0.0.2.dist-info/METADATA
+Filename: boson_sdk-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: boson_sdk-0.0.2.dist-info/WHEEL
+Filename: boson_sdk-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: boson_sdk-0.0.2.dist-info/top_level.txt
+Filename: boson_sdk-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: boson_sdk-0.0.2.dist-info/RECORD
+Filename: boson_sdk-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## boson/__init__.py

```diff
@@ -1,38 +1,32 @@
 import importlib.metadata
 
 from boson.base import BaseProvider
-from boson.boson_v1_pb2 import LandingPageRequest, LandingPageResponse, ConformanceRequest, ConformanceResponse, \
-    CollectionsRequest, CollectionsResponse, CollectionRequest, CollectionResponse, CollectionItemsRequest, \
-    CollectionItemsResponse, CollectionItemRequest, CollectionItemResponse, SearchRequest, SearchResponse, \
-    WarpRequest, RasterResponse
+from boson.boson_v1_pb2 import (
+    DatasetInfoRequest,
+    DatasetInfoResponse,
+    SearchRequest,
+    SearchResponse,
+    WarpRequest,
+    RasterResponse,
+)
 from boson.features_pb2 import CollectionMsg, FeatureMsg, FeatureCollectionMsg, LinkMsg
 
 
 __version__ = importlib.metadata.version("boson-sdk")
 __all__ = [
     "BaseProvider",
-    "LandingPageRequest",
-    "LandingPageResponse",
-    "ConformanceRequest",
-    "ConformanceResponse",
-    "CollectionsRequest",
-    "CollectionsResponse",
-    "CollectionRequest",
-    "CollectionResponse",
-    "CollectionItemsRequest",
-    "CollectionItemsResponse",
-    "CollectionItemRequest",
-    "CollectionItemResponse",
+    "DatasetInfoRequest",
+    "DatasetInfoResponse",
     "SearchRequest",
     "SearchResponse",
     "WarpRequest",
     "RasterResponse",
     "CollectionMsg",
     "FeatureMsg",
     "FeatureCollectionMsg",
     "LinkMsg",
     "search_request_to_kwargs",
     "feature_collection_to_proto",
     "warp_request_to_kwargs",
-    "numpy_to_raster_response"
+    "numpy_to_raster_response",
 ]
```

## boson/base.py

```diff
@@ -1,95 +1,98 @@
 from types import FunctionType
 from typing import Optional
 
-from boson.boson_v1_pb2 import LandingPageResponse, ConformanceRequest, ConformanceResponse, \
-    CollectionsRequest, CollectionsResponse, CollectionRequest, CollectionResponse, WarpRequest, RasterResponse, \
-    SearchRequest, SearchResponse
-from boson.conversion import search_request_to_kwargs, warp_request_to_kwargs, feature_collection_to_proto, \
-    numpy_to_raster_response
+from boson.boson_v1_pb2 import (
+    DatasetInfoRequest,
+    DatasetInfoResponse,
+    WarpRequest,
+    RasterResponse,
+    SearchRequest,
+    SearchResponse,
+)
+from boson.features_pb2 import CollectionMsg
+from boson.conversion import (
+    search_request_to_kwargs,
+    warp_request_to_kwargs,
+    feature_collection_to_proto,
+    numpy_to_raster_response,
+)
 
 
 class BaseProvider:
-    def __init__(self,
-                 title: str = 'remote',
-                 description: str = 'a remote Boson provider',
-                 license: str = '(unknown)',
-                 extent: Optional[dict] = None,
-                 search_func: Optional[FunctionType] = None,
-                 warp_func: Optional[FunctionType] = None) -> None:
-
-        self.title = title
+    def __init__(
+        self,
+        name: str = "remote",
+        alias: str = "Remote Boson Provider",
+        description: str = "a remote Boson provider",
+        license: str = "(unknown)",
+        extent: Optional[dict] = None,
+        search_func: Optional[FunctionType] = None,
+        warp_func: Optional[FunctionType] = None,
+    ) -> None:
+        self.name = name
+        self.alias = alias
         self.description = description
         self.license = license
         self.extent = extent
         if self.extent is None:
             self.extent = {
-                'spatial': {
-                    'bbox': [[-180.0, -90.0, 180.0, 90.0]]
-                },
-                'temporal': {
-                    'interval': [[None, None]]
-                }
+                "spatial": {"bbox": [[-180.0, -90.0, 180.0, 90.0]]},
+                "temporal": {"interval": [[None, None]]},
             }
 
         if search_func is not None and not callable(search_func):
-            raise ValueError('search_func must be a callable or None')
+            raise ValueError("search_func must be a callable or None")
 
         self.search_func = search_func
 
         if warp_func is not None and not callable(warp_func):
-            raise ValueError('warp_func must be a callable or None')
+            raise ValueError("warp_func must be a callable or None")
         self.warp_func = warp_func
         super().__init__()
 
-    def landing_page(self, LandingpageRequest) -> LandingPageResponse:
-        return LandingPageResponse(
-            title=self.title,
-            description=self.description,
-            links=[]
-        )
-
-    def conformance(self, request: ConformanceRequest) -> ConformanceResponse:
-        return ConformanceResponse(
+    def dataset_info(self, _: DatasetInfoRequest) -> DatasetInfoResponse:
+        return DatasetInfoResponse(
+            name=self.name,
+            alias=self.alias,
+            links=[],
             conforms_to=[
-                'https://api.stacspec.org/v1.0.0/core',
-                'https://api.stacspec.org/v1.0.0/item-search',
-                'https://api.stacspec.org/v1.0.0/ogcapi-features',
-                'https://api.stacspec.org/v1.0.0/collections',
-                'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core',
-                'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30',
-                'http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson'
-            ]
+                "https://api.stacspec.org/v1.0.0/core",
+                "https://api.stacspec.org/v1.0.0/item-search",
+                "https://api.stacspec.org/v1.0.0/ogcapi-features",
+                "https://api.stacspec.org/v1.0.0/collections",
+                "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core",
+                "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30",
+                "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson",
+            ],
+            collections=CollectionMsg(**self._collection),
         )
 
-    def collection(self, request: CollectionRequest) -> CollectionResponse:
-        return CollectionResponse(collection=self._collection())
-
-    def collections(self, request: CollectionsRequest) -> CollectionsResponse:
-        return CollectionsResponse(collections=[self._collection()])
-
     def _collection(self) -> dict:
         return {
-            'version': 'v1.0.0',
-            'id': self.title.lower().replace(' ', ''),
-            'title': self.title,
-            'description': self.description,
-            'license': self.license,
+            "version": "v1.0.0",
+            "id": self.name,
+            "title": self.alias,
+            "description": self.description,
+            "license": self.license,
         }
 
     def warp(self, request: WarpRequest) -> RasterResponse:
         warp_kwargs = warp_request_to_kwargs(request)
 
         x = self.warp_func(**warp_kwargs)
 
         return numpy_to_raster_response(x)
 
     def search(self, request: SearchRequest) -> SearchResponse:
         search_kwargs = search_request_to_kwargs(request)
 
-        fc = self.search_func(**search_kwargs)
+        res = self.search_func(**search_kwargs)
+        token = ""
+        if len(res) == 2:
+            fc, token = res
+        else:
+            fc = res
 
         fc_proto = feature_collection_to_proto(fc)
 
-        return SearchResponse(
-            feature_collection=fc_proto
-        )
+        return SearchResponse(feature_collection=fc_proto, token=token)
```

## boson/boson_v1_pb2.py

```diff
@@ -12,58 +12,38 @@
 
 
 import boson.features_pb2 as features__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x62oson_v1.proto\x12\x0f\x62osonproviderv1\x1a\x0e\x66\x65\x61tures.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x12LandingPageRequest\"\x14\n\x12\x43onformanceRequest\"\x14\n\x12\x43ollectionsRequest\"*\n\x11\x43ollectionRequest\x12\x15\n\rcollection_id\x18\x01 \x01(\t\"\xa3\x01\n\x16\x43ollectionItemsRequest\x12\x15\n\rcollection_id\x18\x01 \x01(\t\x12\x0c\n\x04\x62\x62ox\x18\x02 \x03(\x01\x12,\n\x08\x64\x61tetime\x18\x03 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05limit\x18\x05 \x01(\x05\"B\n\x15\x43ollectionItemRequest\x12\x15\n\rcollection_id\x18\x01 \x01(\t\x12\x12\n\nfeature_id\x18\x02 \x01(\t\"\x94\x02\n\rSearchRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12,\n\x08\x64\x61tetime\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x63ollections\x18\x05 \x03(\t\x12\x13\n\x0b\x66\x65\x61ture_ids\x18\x06 \x03(\t\x12\'\n\x06\x66ields\x18\x07 \x01(\x0b\x32\x17.bosonproviderv1.Fields\x12(\n\x07sort_by\x18\x08 \x03(\x0b\x32\x17.bosonproviderv1.SortBy\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nintersects\x18\n \x01(\x0c\"*\n\x06\x46ields\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"*\n\x06SortBy\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\tdirection\x18\x02 \x01(\t\"\xd8\x04\n\x0bWarpRequest\x12\x1f\n\x17input_spatial_reference\x18\x01 \x01(\t\x12 \n\x18output_spatial_reference\x18\x02 \x01(\t\x12\'\n\x1foutput_extent_spatial_reference\x18\x03 \x01(\t\x12\x19\n\x11output_pixel_size\x18\x04 \x03(\x01\x12\x15\n\routput_extent\x18\x05 \x03(\x01\x12\x1b\n\x13output_extent_wgs84\x18\x06 \x03(\x01\x12\x14\n\x0coutput_shape\x18\x07 \x03(\x04\x12\x12\n\npixel_type\x18\x08 \x01(\t\x12\x19\n\x11resampling_method\x18\t \x01(\t\x12-\n\rinput_no_data\x18\n \x03(\x0b\x32\x16.google.protobuf.Value\x12.\n\x0eoutput_no_data\x18\x0b \x03(\x0b\x32\x16.google.protobuf.Value\x12\x14\n\x0c\x63ontent_type\x18\x0c \x01(\t\x12\x30\n\x0ctime_instant\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ntime_range\x18\x0e \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0b\x61sset_bands\x18\x0f \x03(\x0b\x32\x1b.bosonproviderv1.AssetBands\x12\x17\n\x0finput_filepaths\x18\x10 \x03(\t\x12\'\n\x06\x66ilter\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\"C\n\nAssetBands\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12&\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x17.bosonproviderv1.BandID\"\"\n\x06\x42\x61ndID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x05\"W\n\x13LandingPageResponse\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1c\n\x05links\x18\x03 \x03(\x0b\x32\r.gogc.LinkMsg\"*\n\x13\x43onformanceResponse\x12\x13\n\x0b\x63onforms_to\x18\x01 \x03(\t\"=\n\x12\x43ollectionResponse\x12\'\n\ncollection\x18\x01 \x01(\x0b\x32\x13.gogc.CollectionMsg\"?\n\x13\x43ollectionsResponse\x12(\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\x13.gogc.CollectionMsg\"Q\n\x17\x43ollectionItemsResponse\x12\x36\n\x12\x66\x65\x61ture_collection\x18\x01 \x01(\x0b\x32\x1a.gogc.FeatureCollectionMsg\"8\n\x16\x43ollectionItemResponse\x12\x1e\n\x04item\x18\x01 \x01(\x0b\x32\x10.gogc.FeatureMsg\"H\n\x0eSearchResponse\x12\x36\n\x12\x66\x65\x61ture_collection\x18\x01 \x01(\x0b\x32\x1a.gogc.FeatureCollectionMsg\"n\n\x0eRasterResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\r\x12\x12\n\npixel_type\x18\x04 \x01(\t\x12\x15\n\rgeo_transform\x18\x05 \x03(\x01\x32\xe1\x05\n\x0f\x42osonProviderV1\x12Z\n\x0bLandingPage\x12#.bosonproviderv1.LandingPageRequest\x1a$.bosonproviderv1.LandingPageResponse\"\x00\x12Z\n\x0b\x43onformance\x12#.bosonproviderv1.ConformanceRequest\x1a$.bosonproviderv1.ConformanceResponse\"\x00\x12W\n\nCollection\x12\".bosonproviderv1.CollectionRequest\x1a#.bosonproviderv1.CollectionResponse\"\x00\x12Z\n\x0b\x43ollections\x12#.bosonproviderv1.CollectionsRequest\x1a$.bosonproviderv1.CollectionsResponse\"\x00\x12\x66\n\x0f\x43ollectionItems\x12\'.bosonproviderv1.CollectionItemsRequest\x1a(.bosonproviderv1.CollectionItemsResponse\"\x00\x12\x63\n\x0e\x43ollectionItem\x12&.bosonproviderv1.CollectionItemRequest\x1a\'.bosonproviderv1.CollectionItemResponse\"\x00\x12K\n\x06Search\x12\x1e.bosonproviderv1.SearchRequest\x1a\x1f.bosonproviderv1.SearchResponse\"\x00\x12G\n\x04Warp\x12\x1c.bosonproviderv1.WarpRequest\x1a\x1f.bosonproviderv1.RasterResponse\"\x00\x42/Z-github.com/seerai/boson/server/v1/impl/remoteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x62oson_v1.proto\x12\x0f\x62osonproviderv1\x1a\x0e\x66\x65\x61tures.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x14\n\x12\x44\x61tasetInfoRequest\"\xb1\x02\n\rSearchRequest\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\x12,\n\x08\x64\x61tetime\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x63ollections\x18\x05 \x03(\t\x12\x13\n\x0b\x66\x65\x61ture_ids\x18\x06 \x03(\t\x12\'\n\x06\x66ields\x18\x07 \x01(\x0b\x32\x17.bosonproviderv1.Fields\x12(\n\x07sort_by\x18\x08 \x03(\x0b\x32\x17.bosonproviderv1.SortBy\x12\r\n\x05limit\x18\t \x01(\x05\x12\x12\n\nintersects\x18\n \x01(\x0c\x12\x0c\n\x04page\x18\x0b \x01(\x05\x12\r\n\x05token\x18\x0c \x01(\t\"*\n\x06\x46ields\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"*\n\x06SortBy\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\tdirection\x18\x02 \x01(\t\"\xd8\x04\n\x0bWarpRequest\x12\x1f\n\x17input_spatial_reference\x18\x01 \x01(\t\x12 \n\x18output_spatial_reference\x18\x02 \x01(\t\x12\'\n\x1foutput_extent_spatial_reference\x18\x03 \x01(\t\x12\x19\n\x11output_pixel_size\x18\x04 \x03(\x01\x12\x15\n\routput_extent\x18\x05 \x03(\x01\x12\x1b\n\x13output_extent_wgs84\x18\x06 \x03(\x01\x12\x14\n\x0coutput_shape\x18\x07 \x03(\x04\x12\x12\n\npixel_type\x18\x08 \x01(\t\x12\x19\n\x11resampling_method\x18\t \x01(\t\x12-\n\rinput_no_data\x18\n \x03(\x0b\x32\x16.google.protobuf.Value\x12.\n\x0eoutput_no_data\x18\x0b \x03(\x0b\x32\x16.google.protobuf.Value\x12\x14\n\x0c\x63ontent_type\x18\x0c \x01(\t\x12\x30\n\x0ctime_instant\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ntime_range\x18\x0e \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0b\x61sset_bands\x18\x0f \x03(\x0b\x32\x1b.bosonproviderv1.AssetBands\x12\x17\n\x0finput_filepaths\x18\x10 \x03(\t\x12\'\n\x06\x66ilter\x18\x11 \x01(\x0b\x32\x17.google.protobuf.Struct\"C\n\nAssetBands\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12&\n\x05\x62\x61nds\x18\x02 \x03(\x0b\x32\x17.bosonproviderv1.BandID\"\"\n\x06\x42\x61ndID\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x05\"\xf1\x01\n\x13\x44\x61tasetInfoResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\'\n\x0eoverall_extent\x18\x04 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x10\n\x08min_zoom\x18\x05 \x01(\x05\x12\x10\n\x08max_zoom\x18\x06 \x01(\x05\x12\x13\n\x0b\x63onforms_to\x18\x07 \x03(\t\x12\x1c\n\x05links\x18\x08 \x03(\x0b\x32\r.gogc.LinkMsg\x12(\n\x0b\x63ollections\x18\t \x03(\x0b\x32\x13.gogc.CollectionMsg\"W\n\x0eSearchResponse\x12\x36\n\x12\x66\x65\x61ture_collection\x18\x01 \x01(\x0b\x32\x1a.gogc.FeatureCollectionMsg\x12\r\n\x05token\x18\x02 \x01(\t\"n\n\x0eRasterResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\x12\x14\n\x0c\x63ontent_type\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\r\x12\x12\n\npixel_type\x18\x04 \x01(\t\x12\x15\n\rgeo_transform\x18\x05 \x03(\x01\x32\x83\x02\n\x0f\x42osonProviderV1\x12Z\n\x0b\x44\x61tasetInfo\x12#.bosonproviderv1.DatasetInfoRequest\x1a$.bosonproviderv1.DatasetInfoResponse\"\x00\x12K\n\x06Search\x12\x1e.bosonproviderv1.SearchRequest\x1a\x1f.bosonproviderv1.SearchResponse\"\x00\x12G\n\x04Warp\x12\x1c.bosonproviderv1.WarpRequest\x1a\x1f.bosonproviderv1.RasterResponse\"\x00\x42/Z-github.com/seerai/boson/server/v1/impl/remoteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'boson_v1_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z-github.com/seerai/boson/server/v1/impl/remote'
-  _LANDINGPAGEREQUEST._serialized_start=114
-  _LANDINGPAGEREQUEST._serialized_end=134
-  _CONFORMANCEREQUEST._serialized_start=136
-  _CONFORMANCEREQUEST._serialized_end=156
-  _COLLECTIONSREQUEST._serialized_start=158
-  _COLLECTIONSREQUEST._serialized_end=178
-  _COLLECTIONREQUEST._serialized_start=180
-  _COLLECTIONREQUEST._serialized_end=222
-  _COLLECTIONITEMSREQUEST._serialized_start=225
-  _COLLECTIONITEMSREQUEST._serialized_end=388
-  _COLLECTIONITEMREQUEST._serialized_start=390
-  _COLLECTIONITEMREQUEST._serialized_end=456
-  _SEARCHREQUEST._serialized_start=459
-  _SEARCHREQUEST._serialized_end=735
-  _FIELDS._serialized_start=737
-  _FIELDS._serialized_end=779
-  _SORTBY._serialized_start=781
-  _SORTBY._serialized_end=823
-  _WARPREQUEST._serialized_start=826
-  _WARPREQUEST._serialized_end=1426
-  _ASSETBANDS._serialized_start=1428
-  _ASSETBANDS._serialized_end=1495
-  _BANDID._serialized_start=1497
-  _BANDID._serialized_end=1531
-  _LANDINGPAGERESPONSE._serialized_start=1533
-  _LANDINGPAGERESPONSE._serialized_end=1620
-  _CONFORMANCERESPONSE._serialized_start=1622
-  _CONFORMANCERESPONSE._serialized_end=1664
-  _COLLECTIONRESPONSE._serialized_start=1666
-  _COLLECTIONRESPONSE._serialized_end=1727
-  _COLLECTIONSRESPONSE._serialized_start=1729
-  _COLLECTIONSRESPONSE._serialized_end=1792
-  _COLLECTIONITEMSRESPONSE._serialized_start=1794
-  _COLLECTIONITEMSRESPONSE._serialized_end=1875
-  _COLLECTIONITEMRESPONSE._serialized_start=1877
-  _COLLECTIONITEMRESPONSE._serialized_end=1933
-  _SEARCHRESPONSE._serialized_start=1935
-  _SEARCHRESPONSE._serialized_end=2007
-  _RASTERRESPONSE._serialized_start=2009
-  _RASTERRESPONSE._serialized_end=2119
-  _BOSONPROVIDERV1._serialized_start=2122
-  _BOSONPROVIDERV1._serialized_end=2859
+  _DATASETINFOREQUEST._serialized_start=114
+  _DATASETINFOREQUEST._serialized_end=134
+  _SEARCHREQUEST._serialized_start=137
+  _SEARCHREQUEST._serialized_end=442
+  _FIELDS._serialized_start=444
+  _FIELDS._serialized_end=486
+  _SORTBY._serialized_start=488
+  _SORTBY._serialized_end=530
+  _WARPREQUEST._serialized_start=533
+  _WARPREQUEST._serialized_end=1133
+  _ASSETBANDS._serialized_start=1135
+  _ASSETBANDS._serialized_end=1202
+  _BANDID._serialized_start=1204
+  _BANDID._serialized_end=1238
+  _DATASETINFORESPONSE._serialized_start=1241
+  _DATASETINFORESPONSE._serialized_end=1482
+  _SEARCHRESPONSE._serialized_start=1484
+  _SEARCHRESPONSE._serialized_end=1571
+  _RASTERRESPONSE._serialized_start=1573
+  _RASTERRESPONSE._serialized_end=1683
+  _BOSONPROVIDERV1._serialized_start=1686
+  _BOSONPROVIDERV1._serialized_end=1945
 # @@protoc_insertion_point(module_scope)
```

## boson/conversion.py

```diff
@@ -81,15 +81,17 @@
         'bbox': tuple(bbox) if bbox is not None else None,
         'datetime': datetime,
         'filter': filter,
         'collections': collections,
         'feature_ids': feature_ids,
         'fields': fields,
         'intersects': intersects,
-        'limit': request.limit
+        'limit': request.limit,
+        'page': request.page,
+        'token': request.token
     }
 
 
 def numpy_to_raster_response(x: np.ndarray) -> RasterResponse:
     _, descr = x.dtype.descr[0]
 
     return RasterResponse(
```

## boson/features_pb2.py

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xea\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12\x35\n\tsummaries\x18\x0b \x03(\x0b\x32\".gogc.CollectionMsg.SummariesEntry\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1aH\n\x0eSummariesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8b\x03\n\nFeatureMsg\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\t\x12\x10\n\x08geometry\x18\x03 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x04 \x03(\x01\x12\x34\n\nproperties\x18\x05 \x03(\x0b\x32 .gogc.FeatureMsg.PropertiesEntry\x12\x1c\n\x05links\x18\x06 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x07 \x01(\t\x12\x12\n\nextensions\x18\x08 \x03(\t\x12,\n\x06\x61ssets\x18\t \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\n \x01(\t\x1aI\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x04gogc\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xea\x03\n\rCollectionMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x12\x0f\n\x07license\x18\x05 \x01(\t\x12\x1f\n\x06\x65xtent\x18\x06 \x01(\x0b\x32\x0f.gogc.ExtentMsg\x12\x1c\n\x05links\x18\x07 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x08 \x01(\t\x12\x12\n\nextensions\x18\t \x03(\t\x12$\n\tproviders\x18\n \x03(\x0b\x32\x11.gogc.ProviderMsg\x12\x35\n\tsummaries\x18\x0b \x03(\x0b\x32\".gogc.CollectionMsg.SummariesEntry\x12\x38\n\x0bitem_assets\x18\x0c \x03(\x0b\x32#.gogc.CollectionMsg.ItemAssetsEntry\x1aH\n\x0eSummariesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a\x41\n\x0fItemAssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xb8\x01\n\x14\x46\x65\x61tureCollectionMsg\x12\"\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x10.gogc.FeatureMsg\x12\x1c\n\x05links\x18\x02 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x16\n\x0enumber_matched\x18\x03 \x01(\x03\x12\x17\n\x0fnumber_returned\x18\x04 \x01(\x03\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xfd\x02\n\nFeatureMsg\x12\n\n\x02id\x18\x01 \x01(\t\x12\x10\n\x08geometry\x18\x02 \x01(\x0c\x12\x0c\n\x04\x62\x62ox\x18\x03 \x03(\x01\x12\x34\n\nproperties\x18\x04 \x03(\x0b\x32 .gogc.FeatureMsg.PropertiesEntry\x12\x1c\n\x05links\x18\x05 \x03(\x0b\x32\r.gogc.LinkMsg\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x12\n\nextensions\x18\x07 \x03(\t\x12,\n\x06\x61ssets\x18\x08 \x03(\x0b\x32\x1c.gogc.FeatureMsg.AssetsEntry\x12\x12\n\ncollection\x18\t \x01(\t\x1aI\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value:\x02\x38\x01\x1a=\n\x0b\x41ssetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"\xbe\x02\n\x08\x41ssetMsg\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x0c\n\x04href\x18\x04 \x01(\t\x12\r\n\x05roles\x18\x05 \x03(\t\x12!\n\x08\x65o_bands\x18\x06 \x03(\x0b\x32\x0f.gogc.EOBandMsg\x12)\n\x0craster_bands\x18\x07 \x03(\x0b\x32\x13.gogc.RasterBandMsg\x12!\n\x07storage\x18\t \x01(\x0b\x32\x10.gogc.StorageMsg\x12\x30\n\talternate\x18\n \x03(\x0b\x32\x1d.gogc.AssetMsg.AlternateEntry\x1a@\n\x0e\x41lternateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.gogc.AssetMsg:\x02\x38\x01\"T\n\nStorageMsg\x12\x10\n\x08platform\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x16\n\x0erequester_pays\x18\x03 \x01(\x08\x12\x0c\n\x04tier\x18\x04 \x01(\t\"\xa4\x01\n\tEOBandMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x63ommon_name\x18\x02 \x01(\t\x12\x0b\n\x03gsd\x18\x03 \x01(\x01\x12\x19\n\x11\x63\x65nter_wavelength\x18\x04 \x01(\x01\x12\x1b\n\x13\x66ull_width_half_max\x18\x05 \x01(\x01\x12\x1a\n\x12solar_illumination\x18\x06 \x01(\x01\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\"\x9b\x02\n\rRasterBandMsg\x12\'\n\x07no_data\x18\x01 \x01(\x0b\x32\x16.google.protobuf.Value\x12\x10\n\x08sampling\x18\x02 \x01(\t\x12\x11\n\tdata_type\x18\x03 \x01(\t\x12\x17\n\x0f\x62its_per_sample\x18\x04 \x01(\x05\x12\x1a\n\x12spatial_resolution\x18\x05 \x01(\x01\x12-\n\nstatistics\x18\x06 \x01(\x0b\x32\x19.gogc.RasterStatisticsMsg\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\r\n\x05scale\x18\x08 \x01(\x01\x12\x0e\n\x06offset\x18\t \x01(\x01\x12+\n\thistogram\x18\n \x01(\x0b\x32\x18.gogc.RasterHistogramMsg\"l\n\x13RasterStatisticsMsg\x12\x0c\n\x04mean\x18\x01 \x01(\x01\x12\x0f\n\x07minimum\x18\x02 \x01(\x01\x12\x0f\n\x07maximum\x18\x03 \x01(\x01\x12\x0e\n\x06stddev\x18\x04 \x01(\x01\x12\x15\n\rvalid_percent\x18\x05 \x01(\x01\"N\n\x12RasterHistogramMsg\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x0b\n\x03min\x18\x02 \x01(\x01\x12\x0b\n\x03max\x18\x03 \x01(\x01\x12\x0f\n\x07\x62uckets\x18\x04 \x03(\x04\"_\n\tExtentMsg\x12\'\n\x07spatial\x18\x01 \x03(\x0b\x32\x16.gogc.SpatialExtentMsg\x12)\n\x08temporal\x18\x02 \x03(\x0b\x32\x17.gogc.TemporalExtentMsg\" \n\x10SpatialExtentMsg\x12\x0c\n\x04\x62\x62ox\x18\x01 \x03(\x01\"A\n\x11TemporalExtentMsg\x12,\n\x08interval\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x02\n\x07LinkMsg\x12\x0c\n\x04href\x18\x01 \x01(\t\x12\x0b\n\x03rel\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x10\n\x08hreflang\x18\x04 \x01(\t\x12\r\n\x05title\x18\x05 \x01(\t\x12\x0e\n\x06length\x18\x06 \x01(\x03\x12\x0e\n\x06method\x18\x07 \x01(\t\x12+\n\x07headers\x18\x08 \x03(\x0b\x32\x1a.gogc.LinkMsg.HeadersEntry\x12%\n\x04\x62ody\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\r\n\x05merge\x18\n \x01(\x08\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"L\n\x0bProviderMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\x12\x0b\n\x03url\x18\x04 \x01(\tB!Z\x1fgithub.com/seerai/gogc/featuresb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'features_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\037github.com/seerai/gogc/features'
@@ -40,39 +40,39 @@
   _COLLECTIONMSG_SUMMARIESENTRY._serialized_start=439
   _COLLECTIONMSG_SUMMARIESENTRY._serialized_end=511
   _COLLECTIONMSG_ITEMASSETSENTRY._serialized_start=513
   _COLLECTIONMSG_ITEMASSETSENTRY._serialized_end=578
   _FEATURECOLLECTIONMSG._serialized_start=581
   _FEATURECOLLECTIONMSG._serialized_end=765
   _FEATUREMSG._serialized_start=768
-  _FEATUREMSG._serialized_end=1163
-  _FEATUREMSG_PROPERTIESENTRY._serialized_start=1027
-  _FEATUREMSG_PROPERTIESENTRY._serialized_end=1100
-  _FEATUREMSG_ASSETSENTRY._serialized_start=1102
-  _FEATUREMSG_ASSETSENTRY._serialized_end=1163
-  _ASSETMSG._serialized_start=1166
-  _ASSETMSG._serialized_end=1484
-  _ASSETMSG_ALTERNATEENTRY._serialized_start=1420
-  _ASSETMSG_ALTERNATEENTRY._serialized_end=1484
-  _STORAGEMSG._serialized_start=1486
-  _STORAGEMSG._serialized_end=1570
-  _EOBANDMSG._serialized_start=1573
-  _EOBANDMSG._serialized_end=1737
-  _RASTERBANDMSG._serialized_start=1740
-  _RASTERBANDMSG._serialized_end=2023
-  _RASTERSTATISTICSMSG._serialized_start=2025
-  _RASTERSTATISTICSMSG._serialized_end=2133
-  _RASTERHISTOGRAMMSG._serialized_start=2135
-  _RASTERHISTOGRAMMSG._serialized_end=2213
-  _EXTENTMSG._serialized_start=2215
-  _EXTENTMSG._serialized_end=2310
-  _SPATIALEXTENTMSG._serialized_start=2312
-  _SPATIALEXTENTMSG._serialized_end=2344
-  _TEMPORALEXTENTMSG._serialized_start=2346
-  _TEMPORALEXTENTMSG._serialized_end=2411
-  _LINKMSG._serialized_start=2414
-  _LINKMSG._serialized_end=2676
-  _LINKMSG_HEADERSENTRY._serialized_start=2630
-  _LINKMSG_HEADERSENTRY._serialized_end=2676
-  _PROVIDERMSG._serialized_start=2678
-  _PROVIDERMSG._serialized_end=2754
+  _FEATUREMSG._serialized_end=1149
+  _FEATUREMSG_PROPERTIESENTRY._serialized_start=1013
+  _FEATUREMSG_PROPERTIESENTRY._serialized_end=1086
+  _FEATUREMSG_ASSETSENTRY._serialized_start=1088
+  _FEATUREMSG_ASSETSENTRY._serialized_end=1149
+  _ASSETMSG._serialized_start=1152
+  _ASSETMSG._serialized_end=1470
+  _ASSETMSG_ALTERNATEENTRY._serialized_start=1406
+  _ASSETMSG_ALTERNATEENTRY._serialized_end=1470
+  _STORAGEMSG._serialized_start=1472
+  _STORAGEMSG._serialized_end=1556
+  _EOBANDMSG._serialized_start=1559
+  _EOBANDMSG._serialized_end=1723
+  _RASTERBANDMSG._serialized_start=1726
+  _RASTERBANDMSG._serialized_end=2009
+  _RASTERSTATISTICSMSG._serialized_start=2011
+  _RASTERSTATISTICSMSG._serialized_end=2119
+  _RASTERHISTOGRAMMSG._serialized_start=2121
+  _RASTERHISTOGRAMMSG._serialized_end=2199
+  _EXTENTMSG._serialized_start=2201
+  _EXTENTMSG._serialized_end=2296
+  _SPATIALEXTENTMSG._serialized_start=2298
+  _SPATIALEXTENTMSG._serialized_end=2330
+  _TEMPORALEXTENTMSG._serialized_start=2332
+  _TEMPORALEXTENTMSG._serialized_end=2397
+  _LINKMSG._serialized_start=2400
+  _LINKMSG._serialized_end=2662
+  _LINKMSG_HEADERSENTRY._serialized_start=2616
+  _LINKMSG_HEADERSENTRY._serialized_end=2662
+  _PROVIDERMSG._serialized_start=2664
+  _PROVIDERMSG._serialized_end=2740
 # @@protoc_insertion_point(module_scope)
```

## boson/grpc/boson_v1_pb2_grpc.py

```diff
@@ -10,43 +10,18 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.LandingPage = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/LandingPage',
-                request_serializer=boson__v1__pb2.LandingPageRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.LandingPageResponse.FromString,
-                )
-        self.Conformance = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/Conformance',
-                request_serializer=boson__v1__pb2.ConformanceRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.ConformanceResponse.FromString,
-                )
-        self.Collection = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/Collection',
-                request_serializer=boson__v1__pb2.CollectionRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.CollectionResponse.FromString,
-                )
-        self.Collections = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/Collections',
-                request_serializer=boson__v1__pb2.CollectionsRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.CollectionsResponse.FromString,
-                )
-        self.CollectionItems = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/CollectionItems',
-                request_serializer=boson__v1__pb2.CollectionItemsRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.CollectionItemsResponse.FromString,
-                )
-        self.CollectionItem = channel.unary_unary(
-                '/bosonproviderv1.BosonProviderV1/CollectionItem',
-                request_serializer=boson__v1__pb2.CollectionItemRequest.SerializeToString,
-                response_deserializer=boson__v1__pb2.CollectionItemResponse.FromString,
+        self.DatasetInfo = channel.unary_unary(
+                '/bosonproviderv1.BosonProviderV1/DatasetInfo',
+                request_serializer=boson__v1__pb2.DatasetInfoRequest.SerializeToString,
+                response_deserializer=boson__v1__pb2.DatasetInfoResponse.FromString,
                 )
         self.Search = channel.unary_unary(
                 '/bosonproviderv1.BosonProviderV1/Search',
                 request_serializer=boson__v1__pb2.SearchRequest.SerializeToString,
                 response_deserializer=boson__v1__pb2.SearchResponse.FromString,
                 )
         self.Warp = channel.unary_unary(
@@ -55,45 +30,15 @@
                 response_deserializer=boson__v1__pb2.RasterResponse.FromString,
                 )
 
 
 class BosonProviderV1Servicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def LandingPage(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Conformance(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Collection(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def Collections(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CollectionItems(self, request, context):
-        """Missing associated documentation comment in .proto file."""
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
-    def CollectionItem(self, request, context):
+    def DatasetInfo(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Search(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -106,43 +51,18 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_BosonProviderV1Servicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'LandingPage': grpc.unary_unary_rpc_method_handler(
-                    servicer.LandingPage,
-                    request_deserializer=boson__v1__pb2.LandingPageRequest.FromString,
-                    response_serializer=boson__v1__pb2.LandingPageResponse.SerializeToString,
-            ),
-            'Conformance': grpc.unary_unary_rpc_method_handler(
-                    servicer.Conformance,
-                    request_deserializer=boson__v1__pb2.ConformanceRequest.FromString,
-                    response_serializer=boson__v1__pb2.ConformanceResponse.SerializeToString,
-            ),
-            'Collection': grpc.unary_unary_rpc_method_handler(
-                    servicer.Collection,
-                    request_deserializer=boson__v1__pb2.CollectionRequest.FromString,
-                    response_serializer=boson__v1__pb2.CollectionResponse.SerializeToString,
-            ),
-            'Collections': grpc.unary_unary_rpc_method_handler(
-                    servicer.Collections,
-                    request_deserializer=boson__v1__pb2.CollectionsRequest.FromString,
-                    response_serializer=boson__v1__pb2.CollectionsResponse.SerializeToString,
-            ),
-            'CollectionItems': grpc.unary_unary_rpc_method_handler(
-                    servicer.CollectionItems,
-                    request_deserializer=boson__v1__pb2.CollectionItemsRequest.FromString,
-                    response_serializer=boson__v1__pb2.CollectionItemsResponse.SerializeToString,
-            ),
-            'CollectionItem': grpc.unary_unary_rpc_method_handler(
-                    servicer.CollectionItem,
-                    request_deserializer=boson__v1__pb2.CollectionItemRequest.FromString,
-                    response_serializer=boson__v1__pb2.CollectionItemResponse.SerializeToString,
+            'DatasetInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.DatasetInfo,
+                    request_deserializer=boson__v1__pb2.DatasetInfoRequest.FromString,
+                    response_serializer=boson__v1__pb2.DatasetInfoResponse.SerializeToString,
             ),
             'Search': grpc.unary_unary_rpc_method_handler(
                     servicer.Search,
                     request_deserializer=boson__v1__pb2.SearchRequest.FromString,
                     response_serializer=boson__v1__pb2.SearchResponse.SerializeToString,
             ),
             'Warp': grpc.unary_unary_rpc_method_handler(
@@ -157,112 +77,27 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class BosonProviderV1(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def LandingPage(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/LandingPage',
-            boson__v1__pb2.LandingPageRequest.SerializeToString,
-            boson__v1__pb2.LandingPageResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Conformance(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/Conformance',
-            boson__v1__pb2.ConformanceRequest.SerializeToString,
-            boson__v1__pb2.ConformanceResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Collection(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/Collection',
-            boson__v1__pb2.CollectionRequest.SerializeToString,
-            boson__v1__pb2.CollectionResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def Collections(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/Collections',
-            boson__v1__pb2.CollectionsRequest.SerializeToString,
-            boson__v1__pb2.CollectionsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CollectionItems(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/CollectionItems',
-            boson__v1__pb2.CollectionItemsRequest.SerializeToString,
-            boson__v1__pb2.CollectionItemsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
-    def CollectionItem(request,
+    def DatasetInfo(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/CollectionItem',
-            boson__v1__pb2.CollectionItemRequest.SerializeToString,
-            boson__v1__pb2.CollectionItemResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/bosonproviderv1.BosonProviderV1/DatasetInfo',
+            boson__v1__pb2.DatasetInfoRequest.SerializeToString,
+            boson__v1__pb2.DatasetInfoResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Search(request,
             target,
             options=(),
```

## boson/grpc/server.py

```diff
@@ -1,74 +1,65 @@
-
 import os
 import logging
 import grpc
 from types import FunctionType
 from concurrent import futures
 
 from boson import BaseProvider
-from boson.grpc.boson_v1_pb2_grpc import BosonProviderV1Servicer, add_BosonProviderV1Servicer_to_server
-from boson.boson_v1_pb2 import LandingPageRequest, LandingPageResponse, ConformanceRequest, ConformanceResponse, \
-    CollectionsRequest, CollectionsResponse, CollectionRequest, CollectionResponse, CollectionItemsRequest, \
-    CollectionItemsResponse, CollectionItemRequest, CollectionItemResponse, SearchRequest, SearchResponse, \
-    WarpRequest, RasterResponse
+from boson.grpc.boson_v1_pb2_grpc import (
+    BosonProviderV1Servicer,
+    add_BosonProviderV1Servicer_to_server,
+)
+from boson.boson_v1_pb2 import (
+    DatasetInfoRequest,
+    DatasetInfoResponse,
+    SearchRequest,
+    SearchResponse,
+    WarpRequest,
+    RasterResponse,
+)
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(level=logging.INFO)
 
-__all__ = ['serve']
+__all__ = ["serve"]
 
 
 class BosonProviderServicer(BosonProviderV1Servicer, BaseProvider):
-
-    def LandingPage(self, request: LandingPageRequest, context: grpc.ServicerContext) -> LandingPageResponse:
-        return self.landing_page(request)
-
-    def Conformance(self, request: ConformanceRequest, context: grpc.ServicerContext) -> ConformanceResponse:
-        return self.conformance(request)
-
-    def Collections(self, request: CollectionsRequest, context: grpc.ServicerContext) -> CollectionsResponse:
-        return self.collections(request)
-
-    def Collection(self, request: CollectionRequest, context: grpc.ServicerContext) -> CollectionResponse:
-        return self.collection(request)
-
-    def CollectionItems(
-            self, request: CollectionItemsRequest, context: grpc.ServicerContext) -> CollectionItemsResponse:
-        return super().CollectionItem(request, context)
-
-    def CollectionItem(self, request: CollectionItemRequest, context: grpc.ServicerContext) -> CollectionItemResponse:
-        return super().CollectionItem(request, context)
+    def DatasetInfo(
+        self, request: DatasetInfoRequest, context: grpc.ServicerContext
+    ) -> DatasetInfoResponse:
+        return self.dataset_info(request)
 
     def Search(self, request: SearchRequest, context: grpc.ServicerContext) -> SearchResponse:
         try:
             return super().search(request)
         except Exception as e:
-            details = f'unable to run search function: {str(e)}'
+            details = f"unable to run search function: {str(e)}"
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(details)
             return SearchResponse()
 
     def Warp(self, request: WarpRequest, context: grpc.ServicerContext) -> RasterResponse:
         try:
             return super().warp(request)
         except Exception as e:
-            details = f'unable to run warp function: {str(e)}'
+            details = f"unable to run warp function: {str(e)}"
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(details)
             return RasterResponse()
 
 
 def serve(search_func: FunctionType, warp_func: FunctionType, **kwargs) -> grpc.Server:
     logger.info("initializing server")
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=10))
     servicer = BosonProviderServicer(search_func=search_func, warp_func=warp_func, **kwargs)
     add_BosonProviderV1Servicer_to_server(servicer, server)
 
-    port = os.getenv('PROVIDER_PORT')
+    port = os.getenv("PROVIDER_PORT")
     if port is None or port == "":
-        port = '8000'
-    logger.info("initializing starting boson provider server on %s", f'[::]:{port}')
-    server.add_insecure_port(f'[::]:{port}')
+        port = "8000"
+    logger.info("initializing starting boson provider server on %s", f"[::]:{port}")
+    server.add_insecure_port(f"[::]:{port}")
     server.start()
     logger.info("server started")
     server.wait_for_termination()
```

## boson/http/server.py

```diff
@@ -1,110 +1,84 @@
 from typing import Optional, Any
 from types import FunctionType
 from fastapi import FastAPI, APIRouter, Request, Response, HTTPException
-from boson import BaseProvider, LandingPageRequest, ConformanceRequest, CollectionsRequest, CollectionRequest, \
-    WarpRequest, SearchRequest
+from boson import (
+    BaseProvider,
+    DatasetInfoRequest,
+    WarpRequest,
+    SearchRequest,
+)
 
 __all__ = ["serve"]
 
 
 class BosonProvider(BaseProvider):
     def __init__(
-                 self,
-                 title: str = 'remote',
-                 description: str = 'a remote Boson provider',
-                 license: str = '(unknown)',
-                 extent: Optional[dict] = None,
-                 search_func: Optional[FunctionType] = None,
-                 warp_func: Optional[FunctionType] = None) -> None:
-
-        super().__init__(title, description, license, extent, search_func, warp_func)
+        self,
+        name: str = "remote",
+        alias: str = "Remote Boson Provider",
+        description: str = "a remote Boson provider",
+        license: str = "(unknown)",
+        extent: Optional[dict] = None,
+        search_func: Optional[FunctionType] = None,
+        warp_func: Optional[FunctionType] = None,
+    ) -> None:
+        super().__init__(
+            name=name,
+            alias=alias,
+            description=description,
+            license=license,
+            extent=extent,
+            search_func=search_func,
+            warp_func=warp_func,
+        )
 
         self.router = APIRouter()
-        self.router.add_api_route("/", self.landing_page, methods=['POST'])
-        self.router.add_api_route("/conformance", self.conformance, methods=['POST'])
-        self.router.add_api_route("/collections", self.collections, methods=['POST'])
-        self.router.add_api_route("/collection", self.collection, methods=['POST'])
-        self.router.add_api_route("/collection_items", self.collection_items, methods=['POST'])
-        self.router.add_api_route("/collection_item", self.collection_item, methods=['POST'])
-        self.router.add_api_route("/search", self.search, methods=['POST'])
-        self.router.add_api_route("/warp", self.warp, methods=['POST'])
-
-    async def landing_page(self, request: Request):
-        body = await request.body()
-
-        req = LandingPageRequest()
-        req.ParseFromString(body)
+        self.router.add_api_route("/dataset_info", self.dataset_info, methods=["POST"])
+        self.router.add_api_route("/search", self.search, methods=["POST"])
+        self.router.add_api_route("/warp", self.warp, methods=["POST"])
 
-        resp = super().landing_page(req)
-        return self.proto_response(resp)
-
-    async def conformance(self, request: Request):
+    async def dataset_info(self, request: Request):
         body = await request.body()
 
-        req = ConformanceRequest()
+        req = DatasetInfoRequest()
         req.ParseFromString(body)
 
-        resp = super().conformance(req)
+        resp = super().dataset_info(req)
         return self.proto_response(resp)
 
-    async def collections(self, request: Request):
-        body = await request.body()
-
-        req = CollectionsRequest()
-        req.ParseFromString(body)
-
-        resp = super().collections(req)
-        return self.proto_response(resp)
-
-    async def collection(self, request: Request):
-        body = await request.body()
-
-        req = CollectionRequest()
-        req.ParseFromString(body)
-
-        resp = super().collection(req)
-        return self.proto_response(resp)
-
-    async def collection_items(self, request: Request):
-        raise HTTPException(status_code=501, detail='not implemented')
-
-    async def collection_item(self, request: Request):
-        raise HTTPException(status_code=501, detail='not implemented')
-
     async def warp(self, request: Request):
         body = await request.body()
 
         req = WarpRequest()
         req.ParseFromString(body)
 
         try:
             resp = super().warp(req)
         except Exception as e:
-            raise HTTPException(status_code=500, detail=f'unable to run warp function: {str(e)}')
+            raise HTTPException(status_code=500, detail=f"unable to run warp function: {str(e)}")
         return self.proto_response(resp)
 
     async def search(self, request: Request):
         body = await request.body()
 
         req = SearchRequest()
         req.ParseFromString(body)
 
         try:
             resp = super().search(req)
         except Exception as e:
-            raise HTTPException(status_code=500, detail=f'unable to run search function: {str(e)}')
+            raise HTTPException(status_code=500, detail=f"unable to run search function: {str(e)}")
 
         return self.proto_response(resp)
 
     def proto_response(self, resp: Any) -> Response:
-        return Response(
-            content=resp.SerializeToString(),
-            media_type="application/x-protobuf"
-        )
+        return Response(content=resp.SerializeToString(), media_type="application/x-protobuf")
 
 
-def serve(search_func: Optional[FunctionType] = None, warp_func: Optional[FunctionType] = None, **kwargs):
+def serve(
+    search_func: Optional[FunctionType] = None, warp_func: Optional[FunctionType] = None, **kwargs
+):
     app = FastAPI()
     server = BosonProvider(warp_func=warp_func, search_func=search_func, **kwargs)
     app.include_router(server.router)
     return app
```

## Comparing `boson_sdk-0.0.2.dist-info/LICENSE` & `boson_sdk-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `boson_sdk-0.0.2.dist-info/METADATA` & `boson_sdk-0.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boson-sdk
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python SDK for Boson Geospatial Service Mesh Providers
 Author-email: The SeerAI Team <contact@seer.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `boson_sdk-0.0.2.dist-info/RECORD` & `boson_sdk-0.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-boson/__init__.py,sha256=2zfZHZG40i8b-fZ9MFtaGFTfTQlhO4dAPVsU4V6Kp8c,1231
-boson/base.py,sha256=SSEuNJhj3iLwTzKJ1re10b5EZOtF1u5Jew2lNPiZ72Q,3518
-boson/boson_v1_pb2.py,sha256=dsjJ-lDWr3YSyeIWotDFKjBpYK5mN_m0uGav98UqaNk,7430
-boson/conversion.py,sha256=oBsrISYAJswBaqcbgo5Vqwt3HStY6pj7zvqMIKcJgtU,3652
-boson/features_pb2.py,sha256=z68eDG5TXnHkAmlw0MxVAnS-iMuNzQ_lbd9pyQ-SiyQ,8528
+boson/__init__.py,sha256=Xnoa1_beJWNJ7vMFMhJdJM3cMKOQzvK0cwnlh7GsprA,749
+boson/base.py,sha256=8wEWKFirWB4I46hOFslUFd6Le9YwmCwrXVbw83WbQ6k,3157
+boson/boson_v1_pb2.py,sha256=3SDZu0ktfhwRGkjrXDliI_uOQIYgZnqvGSTnF3Z7SEE,5320
+boson/conversion.py,sha256=WxminEDzcwj0o3txCi10bNc87d3GSH17htTXtVtevF4,3714
+boson/features_pb2.py,sha256=VFTKLcXxvSfqnuW_-Sj1qR6FiXrG33PzssSOAdx6Ads,8496
 boson/grpc/__init__.py,sha256=Z1VcMBg4TgrsHfO7jI7pyAZ0jKzJ1ya4gn5gwJkYGp8,57
-boson/grpc/boson_v1_pb2_grpc.py,sha256=J2yn9WOd8hDBak4lqW5L5Tsfu8wOoDHF2smzdcOE7tM,13436
-boson/grpc/server.py,sha256=7BKNDwDhtAMlrJG12bEPYvS6rWPR0xkUlkUKtOFDdUo,3160
+boson/grpc/boson_v1_pb2_grpc.py,sha256=aL02_ezWzSWJIDy5n2mxCswmGA4bMyXbGkU6FURivGo,5518
+boson/grpc/server.py,sha256=XBMosGe56I827E00QGUsIngyZiWUyfAo0hbDNFamYLA,2159
 boson/http/__init__.py,sha256=1J3MipaATnk1VFxmMV0uXeW7DWrD9t6vfcDlHOEjyrA,57
-boson/http/server.py,sha256=t9J6Xin4xH6tOv5ePox4_G36AA2Ulzvly5h2tbSr4R8,3898
-boson_sdk-0.0.2.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
-boson_sdk-0.0.2.dist-info/METADATA,sha256=nFSMGDJxFLaUcaswxB8HYgx8b9olM5jtvr2MHlAzQdE,14911
-boson_sdk-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-boson_sdk-0.0.2.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
-boson_sdk-0.0.2.dist-info/RECORD,,
+boson/http/server.py,sha256=Q2gKtPCyXenaxNRUNkZF28FvuzcqRmtDLICA-Wrbx6k,2568
+boson_sdk-0.1.0.dist-info/LICENSE,sha256=QwcOLU5TJoTeUhuIXzhdCEEDDvorGiC6-3YTOl4TecE,11356
+boson_sdk-0.1.0.dist-info/METADATA,sha256=E7ReiCEYNZS_ZKFGqEJQoM63OzBWxfoj9pHTwyTWCKo,14911
+boson_sdk-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+boson_sdk-0.1.0.dist-info/top_level.txt,sha256=a05hL1bKBp1M9A2czOQcnAZrKe63bhOjgjTAf4ri-4c,6
+boson_sdk-0.1.0.dist-info/RECORD,,
```

