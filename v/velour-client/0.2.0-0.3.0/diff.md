# Comparing `tmp/velour-client-0.2.0.tar.gz` & `tmp/velour-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velour-client-0.2.0.tar", last modified: Fri May 19 18:22:35 2023, max compression
+gzip compressed data, was "velour-client-0.3.0.tar", last modified: Thu Jun  1 18:29:32 2023, max compression
```

## Comparing `velour-client-0.2.0.tar` & `velour-client-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:22:35.428936 velour-client-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-19 18:22:24.000000 velour-client-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 18:22:35.428936 velour-client-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-19 18:22:24.000000 velour-client-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-19 18:22:24.000000 velour-client-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 18:22:35.428936 velour-client-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-19 18:22:24.000000 velour-client-0.2.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:22:35.424935 velour-client-0.2.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-19 18:22:24.000000 velour-client-0.2.0/unit-tests/test_yolo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:22:35.424935 velour-client-0.2.0/velour/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27670 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:22:35.424935 velour-client-0.2.0/velour/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/integrations/chariot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/integrations/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/integrations/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-19 18:22:24.000000 velour-client-0.2.0/velour/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 18:22:35.428936 velour-client-0.2.0/velour_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-19 18:22:35.000000 velour-client-0.2.0/velour_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-19 18:22:35.000000 velour-client-0.2.0/velour_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 18:22:35.000000 velour-client-0.2.0/velour_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-19 18:22:35.000000 velour-client-0.2.0/velour_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-19 18:22:35.000000 velour-client-0.2.0/velour_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-01 18:29:23.000000 velour-client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 18:29:32.983302 velour-client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 18:29:23.000000 velour-client-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-01 18:29:23.000000 velour-client-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:29:32.983302 velour-client-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-01 18:29:23.000000 velour-client-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.979303 velour-client-0.3.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-01 18:29:23.000000 velour-client-0.3.0/unit-tests/test_yolo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.979303 velour-client-0.3.0/velour/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28176 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/velour/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    14911 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/chariot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/integrations/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-06-01 18:29:23.000000 velour-client-0.3.0/velour/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:29:32.983302 velour-client-0.3.0/velour_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 18:29:32.000000 velour-client-0.3.0/velour_client.egg-info/top_level.txt
```

### Comparing `velour-client-0.2.0/LICENSE` & `velour-client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/PKG-INFO` & `velour-client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.2.0/pyproject.toml` & `velour-client-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/unit-tests/test_chariot.py` & `velour-client-0.3.0/unit-tests/test_chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/unit-tests/test_client.py` & `velour-client-0.3.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/unit-tests/test_coco.py` & `velour-client-0.3.0/unit-tests/test_coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/unit-tests/test_data_types.py` & `velour-client-0.3.0/unit-tests/test_data_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from velour.data_types import (
     BoundingBox,
     BoundingPolygon,
     GroundTruthDetection,
     GroundTruthInstanceSegmentation,
     GroundTruthSemanticSegmentation,
     Label,
+    Metadatum,
     PredictedDetection,
     PredictedImageClassification,
     ScoredLabel,
     _GroundTruthSegmentation,
 )
 
 
@@ -134,7 +135,17 @@
     assert PredictedImageClassification(
         image=None,
         scored_labels=[
             ScoredLabel(label=Label("k", "v1"), score=0.2),
             ScoredLabel(label=Label("k", "v2"), score=0.8),
         ],
     )
+
+
+def test_metadatum_validation():
+    md = Metadatum(name="name", value={"a": 3})
+    assert md.value == {"a": 3}
+
+    with pytest.raises(ValueError) as exc_info:
+        Metadatum(name="", value={"a": {3}})
+
+    assert "must be valid GeoJSON" in str(exc_info)
```

### Comparing `velour-client-0.2.0/unit-tests/test_viz.py` & `velour-client-0.3.0/unit-tests/test_viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/unit-tests/test_yolo.py` & `velour-client-0.3.0/unit-tests/test_yolo.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,17 +259,17 @@
     assert len(predictions) == bboxes.shape[0]
     for i in range(len(predictions)):
         assert isinstance(predictions[i], PredictedInstanceSegmentation)
         assert predictions[i].image.uid == image["uid"]
         assert predictions[i].image.height == image["height"]
         assert predictions[i].image.width == image["width"]
         assert predictions[i].image.frame is None
-        assert predictions[i].scored_labels.label.key == "class_label"
-        assert predictions[i].scored_labels.label.value == names[i]
-        assert predictions[i].scored_labels.score == bboxes[i][4]
+        assert predictions[i].scored_labels[0].label.key == "class_label"
+        assert predictions[i].scored_labels[0].label.value == names[i]
+        assert predictions[i].scored_labels[0].score == bboxes[i][4]
         assert predictions[i].mask.shape == velour_mask.shape
         assert (predictions[i].mask == velour_mask).all()
 
 
 def test_parse_yolo_object_detection(image, bboxes, names):
     img = numpy.random.rand(image["height"], image["width"], 3)
 
@@ -282,14 +282,14 @@
     assert len(predictions) == bboxes.shape[0]
     for i in range(len(predictions)):
         assert isinstance(predictions[i], PredictedDetection)
         assert predictions[i].image.uid == image["uid"]
         assert predictions[i].image.height == image["height"]
         assert predictions[i].image.width == image["width"]
         assert predictions[i].image.frame is None
-        assert predictions[i].scored_labels.label.key == "class_label"
-        assert predictions[i].scored_labels.label.value == names[i]
-        assert predictions[i].scored_labels.score == bboxes[i][4]
+        assert predictions[i].scored_labels[0].label.key == "class_label"
+        assert predictions[i].scored_labels[0].label.value == names[i]
+        assert predictions[i].scored_labels[0].score == bboxes[i][4]
         assert predictions[i].bbox.xmin == bboxes[i][0]
         assert predictions[i].bbox.ymin == bboxes[i][1]
         assert predictions[i].bbox.xmax == bboxes[i][2]
         assert predictions[i].bbox.ymax == bboxes[i][3]
```

### Comparing `velour-client-0.2.0/velour/client.py` & `velour-client-0.3.0/velour/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     BoundingPolygon,
     GroundTruthDetection,
     GroundTruthImageClassification,
     GroundTruthInstanceSegmentation,
     GroundTruthSemanticSegmentation,
     Image,
     Label,
+    Metadatum,
     Point,
     PolygonWithHole,
     PredictedDetection,
     PredictedImageClassification,
     ScoredLabel,
     _GroundTruthSegmentation,
     _PredictedSegmentation,
@@ -132,28 +133,43 @@
 
     def delete(self):
         return self.client.delete_dataset(self.name)
 
 
 class TabularDataset(DatasetBase):
     def add_groundtruth(
-        self, groundtruth: Union[List[List[Label]], Dict[str, List[Label]]]
+        self,
+        groundtruth: Union[
+            List[List[Union[Label, Metadatum]]],
+            Dict[str, List[Union[Label, Metadatum]]],
+        ],
     ):
         if isinstance(groundtruth, list):
             # make uids the list indices (as strings)
             groundtruth = {str(i): gt for i, gt in enumerate(groundtruth)}
 
         payload = {
             "dataset_name": self.name,
             "classifications": [
                 {
-                    "labels": [asdict(label) for label in labels],
-                    "datum": {"uid": uid},
+                    "labels": [
+                        asdict(x)
+                        for x in labels_and_metadata
+                        if isinstance(x, Label)
+                    ],
+                    "datum": {
+                        "uid": uid,
+                        "metadata": [
+                            asdict(x)
+                            for x in labels_and_metadata
+                            if isinstance(x, Metadatum)
+                        ],
+                    },
                 }
-                for uid, labels in groundtruth.items()
+                for uid, labels_and_metadata in groundtruth.items()
             ],
         }
 
         resp = self.client._requests_post_rel_host(
             "groundtruth-classifications", json=payload
         )
 
@@ -485,15 +501,15 @@
     ):
         log = []
 
         if not isinstance(predictions, list):
             raise ValueError("GroundTruth argument should be a list.")
 
         if len(predictions) == 0:
-            raise ValueError("Empty list.")
+            return []
 
         for chunk in _generate_chunks(
             self.name,
             predictions,
             chunk_size=chunk_size,
             progress_bar_title="Uploading",
             show_progress_bar=show_progress_bar,
@@ -760,26 +776,26 @@
             },
         )
 
         return class_(client=self, name=name)
 
     def create_image_dataset(
         self, name: str, href: str = None, description: str = None
-    ):
+    ) -> ImageDataset:
         return self._create_model_or_dataset(
             entity_type="datasets",
             datum_type=DatumTypes.IMAGE,
             name=name,
             href=href,
             description=description,
         )
 
     def create_tabular_dataset(
         self, name: str, href: str = None, description: str = None
-    ):
+    ) -> TabularDataset:
         return self._create_model_or_dataset(
             entity_type="datasets",
             datum_type=DatumTypes.TABULAR,
             name=name,
             href=href,
             description=description,
         )
```

### Comparing `velour-client-0.2.0/velour/data_types.py` & `velour-client-0.3.0/velour/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+import json
 from abc import ABC
 from dataclasses import dataclass, field
 from typing import List, Tuple, Union
 
 import numpy as np
 
 
 @dataclass
+class Metadatum:
+    name: str
+    value: Union[float, str, dict]
+
+    def __post_init__(self):
+        if isinstance(self.value, dict):
+            # check that the dict is JSON serializable
+            try:
+                json.dumps(self.value)
+            except TypeError:
+                raise ValueError(
+                    f"if a dict, `value` must be valid GeoJSON but got {self.value}"
+                )
+
+
+@dataclass
 class Image:
     uid: str
     height: int
     width: int
     frame: int = None
+    metadata: List[Metadatum] = field(default_factory=list)
 
 
 @dataclass
 class Label:
     key: str
     value: str
```

### Comparing `velour-client-0.2.0/velour/integrations/chariot.py` & `velour-client-0.3.0/velour/integrations/chariot.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/velour/integrations/coco.py` & `velour-client-0.3.0/velour/integrations/coco.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/velour/integrations/yolo.py` & `velour-client-0.3.0/velour/integrations/yolo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from pathlib import Path
 from typing import Union
 
 import numpy
 import PIL
 from PIL.Image import Resampling
 
-from velour.client import Client, ImageModel
 from velour.data_types import (
     BoundingBox,
     Image,
     Label,
     PredictedDetection,
     PredictedImageClassification,
     PredictedInstanceSegmentation,
@@ -92,15 +90,15 @@
         )
         for raw in result.masks.data
     ]
 
     return [
         PredictedInstanceSegmentation(
             mask=mask,
-            scored_labels=scored_label,
+            scored_labels=[scored_label],
             image=Image(
                 uid=image_uid,
                 height=image_height,
                 width=image_width,
             ),
         )
         for mask, scored_label in list(zip(masks, scored_labels))
@@ -126,25 +124,25 @@
         )
         for label, probability in list(zip(labels, probabilities))
     ]
 
     # Extract Bounding Boxes
     bboxes = [
         BoundingBox(
-            xmin=box[0],
-            ymin=box[1],
-            xmax=box[2],
-            ymax=box[3],
+            xmin=int(box[0]),
+            ymin=int(box[1]),
+            xmax=int(box[2]),
+            ymax=int(box[3]),
         )
         for box in bboxes
     ]
 
     return [
         PredictedDetection(
-            scored_labels=scored_label,
+            scored_labels=[scored_label],
             image=Image(
                 uid=image_uid,
                 height=image_height,
                 width=image_width,
             ),
             bbox=bbox,
         )
```

### Comparing `velour-client-0.2.0/velour/viz.py` & `velour-client-0.3.0/velour/viz.py`

 * *Files identical despite different names*

### Comparing `velour-client-0.2.0/velour_client.egg-info/PKG-INFO` & `velour-client-0.3.0/velour_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: velour-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python client for the Velour evaluation store
 License: Copyright 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
```

### Comparing `velour-client-0.2.0/velour_client.egg-info/SOURCES.txt` & `velour-client-0.3.0/velour_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

