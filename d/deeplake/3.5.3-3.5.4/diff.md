# Comparing `tmp/deeplake-3.5.3.tar.gz` & `tmp/deeplake-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.5.3.tar", last modified: Fri May 26 16:31:42 2023, max compression
+gzip compressed data, was "deeplake-3.5.4.tar", last modified: Thu Jun  1 16:59:07 2023, max compression
```

## Comparing `deeplake-3.5.3.tar` & `deeplake-3.5.4.tar`

### file list

```diff
@@ -1,394 +1,394 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.883961 deeplake-3.5.3/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-05-26 16:30:01.000000 deeplake-3.5.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-26 16:30:01.000000 deeplake-3.5.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25286 2023-05-26 16:31:42.883961 deeplake-3.5.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24579 2023-05-26 16:30:01.000000 deeplake-3.5.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.813961 deeplake-3.5.3/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94609 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    81579 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     6352 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.823961 deeplake-3.5.3/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19270 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.833961 deeplake-3.5.3/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   109420 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170900 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11464 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.843961 deeplake-3.5.3/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25686 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    49384 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    11475 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51192 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29318 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      509 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12123 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)     4993 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8071 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     7799 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.853961 deeplake-3.5.3/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6781 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25905 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22441 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.863961 deeplake-3.5.3/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4072 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.873961 deeplake-3.5.3/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4477 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34711 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.873961 deeplake-3.5.3/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4206 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.883961 deeplake-3.5.3/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25208 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.883961 deeplake-3.5.3/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-05-26 16:30:01.000000 deeplake-3.5.3/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 16:31:42.813961 deeplake-3.5.3/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25286 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12524 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-26 16:31:42.000000 deeplake-3.5.3/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-05-26 16:31:42.883961 deeplake-3.5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-05-26 16:30:01.000000 deeplake-3.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-01 16:57:59.000000 deeplake-3.5.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 16:57:59.000000 deeplake-3.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    25286 2023-06-01 16:59:07.610155 deeplake-3.5.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    24579 2023-06-01 16:57:59.000000 deeplake-3.5.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94609 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    84314 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7389 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19270 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     6262 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   113290 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   170900 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14805 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    11242 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    19976 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      441 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50140 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12386 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51192 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29318 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      509 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12123 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)     5044 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     7799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3147 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3352 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6781 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5463 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    15328 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34711 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3914 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25208 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    25286 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12524 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      978 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-01 16:59:07.610155 deeplake-3.5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-06-01 16:57:59.000000 deeplake-3.5.4/setup.py
```

### Comparing `deeplake-3.5.3/LICENSE` & `deeplake-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/PKG-INFO` & `deeplake-3.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.3
+Version: 3.5.4
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
@@ -314,15 +314,15 @@
 
 </details>
 
 
 <details>
   <summary><b>Deep Lake vs Pinecone</b></summary>
   
-Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring search for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
 
 </details>
 
 <details>
   <summary><b>Deep Lake vs Weaviate</b></summary>
   
 Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.3 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.5.4 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
@@ -159,15 +159,15 @@
 embeddings. ChromaDB is limited to light metadata on top of the embeddings and
 has no visualization. Deep Lake datasets can be visualized and version
 controlled. Deep Lake also has a performant dataloader for fine-tuning your
 Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
 enable users to store and search vectors (embeddings) and offer integrations
 with LangChain and LlamaIndex. However, they are architecturally very
 different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring serach for billions of vectors. Deep
+highly demanding applications requiring search for billions of vectors. Deep
 Lake is a serverless. All computations run client-side, which enables users to
 get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
 raw data such as images, videos, and text, in addition to embeddings. Deep Lake
 datasets can be visualized and version controlled. Pinecone is limited to light
 metadata on top of the embeddings and has no visualization. Deep Lake also has
 a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
 vs Weaviate Both Deep Lake and Weaviate enable users to store and search
```

### Comparing `deeplake-3.5.3/README.md` & `deeplake-3.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
 </details>
 
 
 <details>
   <summary><b>Deep Lake vs Pinecone</b></summary>
   
-Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring search for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
 
 </details>
 
 <details>
   <summary><b>Deep Lake vs Weaviate</b></summary>
   
 Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models.
```

#### html2text {}

```diff
@@ -149,15 +149,15 @@
 embeddings. ChromaDB is limited to light metadata on top of the embeddings and
 has no visualization. Deep Lake datasets can be visualized and version
 controlled. Deep Lake also has a performant dataloader for fine-tuning your
 Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
 enable users to store and search vectors (embeddings) and offer integrations
 with LangChain and LlamaIndex. However, they are architecturally very
 different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring serach for billions of vectors. Deep
+highly demanding applications requiring search for billions of vectors. Deep
 Lake is a serverless. All computations run client-side, which enables users to
 get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
 raw data such as images, videos, and text, in addition to embeddings. Deep Lake
 datasets can be visualized and version controlled. Pinecone is limited to light
 metadata on top of the embeddings and has no visualization. Deep Lake also has
 a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
 vs Weaviate Both Deep Lake and Weaviate enable users to store and search
```

### Comparing `deeplake-3.5.3/deeplake/__init__.py` & `deeplake-3.5.4/deeplake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.5.3"
+__version__ = "3.5.4"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.5.3/deeplake/api/dataset.py` & `deeplake-3.5.4/deeplake/api/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/info.py` & `deeplake-3.5.4/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/link.py` & `deeplake-3.5.4/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/link_tiled.py` & `deeplake-3.5.4/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/read.py` & `deeplake-3.5.4/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_access_method.py` & `deeplake-3.5.4/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_agreement.py` & `deeplake-3.5.4/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_api.py` & `deeplake-3.5.4/deeplake/api/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2519,7 +2519,86 @@
     ds["x/y/z"].extend(list(range(100)))
 
     for i, sample in enumerate(ds):
         assert sample["x/y"].z.is_iteration == True
 
     for i, sample in enumerate(ds):
         assert sample["x/y/z"].is_iteration == True
+
+
+def test_shapes(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        np.testing.assert_array_equal(ds.abc.shapes(), np.zeros((0, 0)))
+
+        ds.abc.append(np.ones((3, 4)))
+        ds.abc.append(np.ones((5, 6)))
+        np.testing.assert_array_equal(ds.abc.shapes(), np.array([[3, 4], [5, 6]]))
+
+        ds.abc.append(None)
+        np.testing.assert_array_equal(
+            ds.abc.shapes(), np.array([[3, 4], [5, 6], [0, 0]])
+        )
+
+        ds.abc.append([])
+        np.testing.assert_array_equal(
+            ds.abc.shapes(), np.array([[3, 4], [5, 6], [0, 0], [0, 0]])
+        )
+
+        with pytest.raises(SampleAppendError):
+            ds.abc.append(np.ones((3, 4, 5)))
+
+        ds.abc.append(np.ones((4, 6)))
+        np.testing.assert_array_equal(
+            ds.abc.shapes(), np.array([[3, 4], [5, 6], [0, 0], [0, 0], [4, 6]])
+        )
+
+        np.testing.assert_array_equal(ds.abc[0].shapes(), np.array([[3, 4]]))
+        np.testing.assert_array_equal(
+            ds.abc[1:4].shapes(), np.array([[5, 6], [0, 0], [0, 0]])
+        )
+        np.testing.assert_array_equal(ds.abc[1::2].shapes(), np.array([[5, 6], [0, 0]]))
+
+
+def test_shapes_sequence(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc", htype="sequence")
+        np.testing.assert_array_equal(ds.abc.shapes(), np.zeros((0, 0)))
+
+        ds.abc.append([np.ones((3, 4)), np.ones((4, 5))])
+        np.testing.assert_array_equal(ds.abc.shapes(), np.array([[[3, 4], [4, 5]]]))
+
+        ds.abc.append([np.ones((2, 3)), np.ones((3, 4))])
+        np.testing.assert_array_equal(
+            ds.abc.shapes(), np.array([[[3, 4], [4, 5]], [[2, 3], [3, 4]]])
+        )
+
+        ds.abc.append([None, None])
+        np.testing.assert_array_equal(
+            ds.abc.shapes(),
+            np.array([[[3, 4], [4, 5]], [[2, 3], [3, 4]], [[0, 0], [0, 0]]]),
+        )
+
+        ds.abc.append([np.ones((2, 3)), np.ones((3, 4)), None])
+        shapes = [
+            np.array([[3, 4], [4, 5]]),
+            np.array([[2, 3], [3, 4]]),
+            np.array([[0, 0], [0, 0]]),
+            np.array([[2, 3], [3, 4], [0, 0]]),
+        ]
+        for i, shape in enumerate(ds.abc.shapes()):
+            np.testing.assert_array_equal(shape, shapes[i])
+
+        np.testing.assert_array_equal(ds.abc[0].shapes(), np.array([[[3, 4], [4, 5]]]))
+        np.testing.assert_array_equal(
+            ds.abc[:3].shapes(),
+            np.array([[[3, 4], [4, 5]], [[2, 3], [3, 4]], [[0, 0], [0, 0]]]),
+        )
+
+
+def test_shape_squeeze(memory_ds):
+    with memory_ds as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend(np.ones((5, 10, 10, 10)))
+        ds.abc.extend(np.ones((5, 10, 12, 20)))
+
+    assert ds.abc[5:, :, 9].shape == (5, 10, 20)
```

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.5.4/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.5.4/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.5.4/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.5.4/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_dataset.py` & `deeplake-3.5.4/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_dicom.py` & `deeplake-3.5.4/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_downsample.py` & `deeplake-3.5.4/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_events.py` & `deeplake-3.5.4/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_grayscale.py` & `deeplake-3.5.4/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_info.py` & `deeplake-3.5.4/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.5.4/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_json.py` & `deeplake-3.5.4/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_link.py` & `deeplake-3.5.4/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.5.4/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_linking.py` & `deeplake-3.5.4/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_mesh.py` & `deeplake-3.5.4/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_meta.py` & `deeplake-3.5.4/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_nifti.py` & `deeplake-3.5.4/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_none.py` & `deeplake-3.5.4/deeplake/api/tests/test_none.py`

 * *Files 18% similar despite different names*

```diff
@@ -159,7 +159,68 @@
         assert ds.xyz[0].numpy().tolist() == []
         assert ds.xyz[1].numpy().shape == (0,)
         assert ds.xyz[1].shape == (0,)
         assert ds.xyz[1].numpy().tolist() == []
         assert ds.xyz[2].numpy().shape == (2,)
         assert ds.xyz[2].shape == (2,)
         assert ds.xyz[2].numpy().tolist() == ["hello", "world"]
+
+
+def test_none_bugs(local_ds):
+    with local_ds as ds:
+        ds.create_tensor("abc")
+        ds.abc.extend(
+            [
+                None,
+                np.array([80, 22, 1]),
+                None,
+                np.array([0, 565, 234]),
+            ]
+        )
+
+        ds.create_tensor("xyz", dtype="int64")
+        ds.xyz.extend(
+            [
+                None,
+                np.array([80, 22, 1]),
+                None,
+                np.array([0, 565, 234]),
+            ]
+        )
+
+    assert ds.abc.htype == "generic"
+    assert ds.xyz.htype == "generic"
+    assert ds.xyz.dtype == np.dtype("int64")
+
+    with local_ds as ds:
+        ds.create_tensor("dummy1")
+        ds.dummy1.extend(
+            np.array(
+                [None, np.array([80, 22, 1]), None, np.array([0, 565, 234])],
+                dtype=object,
+            )
+        )
+
+        ds.create_tensor("dummy2", dtype="int64")
+        ds.dummy2.extend(
+            np.array(
+                [None, np.array([80, 22, 1]), None, np.array([0, 565, 234])],
+                dtype=object,
+            )
+        )
+
+    expected = [
+        np.array([]),
+        np.array([80, 22, 1]),
+        np.array([]),
+        np.array([0, 565, 234]),
+    ]
+    res = ds.dummy1.numpy(aslist=True)
+
+    for i in range(len(expected)):
+        np.testing.assert_array_equal(expected[i], res[i])
+
+    assert ds.dummy2.dtype == np.dtype("int64")
+    res = ds.dummy2.numpy(aslist=True)
+
+    for i in range(len(expected)):
+        np.testing.assert_array_equal(expected[i], res[i])
```

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.5.4/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_pickle.py` & `deeplake-3.5.4/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.5.4/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_polygons.py` & `deeplake-3.5.4/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_pop.py` & `deeplake-3.5.4/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_readonly.py` & `deeplake-3.5.4/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_rechunk.py` & `deeplake-3.5.4/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_reset.py` & `deeplake-3.5.4/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_sample_info.py` & `deeplake-3.5.4/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_text.py` & `deeplake-3.5.4/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_update_samples.py` & `deeplake-3.5.4/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_video.py` & `deeplake-3.5.4/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tests/test_views.py` & `deeplake-3.5.4/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/api/tiled.py` & `deeplake-3.5.4/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/structured/base.py` & `deeplake-3.5.4/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/structured/dataframe.py` & `deeplake-3.5.4/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.5.4/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.5.4/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.5.4/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.5.4/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/base.py` & `deeplake-3.5.4/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.5.4/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.5.4/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.5.4/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.5.4/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.5.4/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.5.4/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/util.py` & `deeplake-3.5.4/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.5.4/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.5.4/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/cli/auth.py` & `deeplake-3.5.4/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/cli/test_cli.py` & `deeplake-3.5.4/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/client/client.py` & `deeplake-3.5.4/deeplake/client/client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/client/config.py` & `deeplake-3.5.4/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/client/log.py` & `deeplake-3.5.4/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/client/test_client.py` & `deeplake-3.5.4/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/client/utils.py` & `deeplake-3.5.4/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/compression.py` & `deeplake-3.5.4/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/constants.py` & `deeplake-3.5.4/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/base_chunk.py` & `deeplake-3.5.4/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.5.4/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.5.4/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.5.4/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.5.4/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.5.4/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.5.4/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/chunk_engine.py` & `deeplake-3.5.4/deeplake/core/chunk_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -687,15 +687,17 @@
             ]
         verified_samples = self.check_each_sample(samples, verify=verify)
         tensor_meta = self.tensor_meta
         all_empty = all(sample is None for sample in samples)
         if tensor_meta.htype is None and not all_empty:
             tensor_meta.set_htype(get_htype(samples))
         if tensor_meta.dtype is None and not all_empty:
-            tensor_meta.set_dtype(get_dtype(samples[0]))
+            tensor_meta.set_dtype(
+                get_dtype(next(filter(lambda x: x is not None, samples)))
+            )  # first non empty sample
         if self._convert_to_list(samples):
             samples = list(samples)
         if self._is_temp_label_tensor:
             samples = verified_samples = convert_to_hash(samples, self._hash_label_map)
         elif tensor_meta.htype in ("image.gray", "image.rgb"):
             mode = "L" if tensor_meta.htype == "image.gray" else "RGB"
             converted = []
@@ -2491,114 +2493,231 @@
             elif length > max_:
                 max_ = length
         return min_, max_
 
     def check_link_ready(self):
         return
 
-    def shape(
+    def _get_sample_shape_from_provider(
+        self, sample_shape_provider, idx, sample_index, flatten
+    ):
+        try:
+            shape = sample_shape_provider(idx)  # type: ignore
+        except (
+            IndexError
+        ):  # Happens during transforms, sample shape tensor is not populated yet
+            shape = self.read_shape_for_sample(idx)  # type: ignore
+
+        if isinstance(shape, tuple) and shape == ():
+            shape = (0,)
+        if self.is_sequence and not flatten:
+            shape = self._merge_seq_shape(shape, sample_index)
+        return shape
+
+    def _merge_seq_shape(self, shape, sample_index):
+        """Merges shapes of sequence items into one shape"""
+        if sample_index and not sample_index[0].subscriptable():
+            shape = (1, *tuple(shape[sample_index[0].value].tolist()))  # type: ignore
+        else:
+            is_same = np.all(shape == shape[0, :], axis=0)  # type: ignore
+            shape = (len(shape),) + (
+                tuple(
+                    int(shape[0, i])  # type: ignore
+                    if is_same[i]  # type: ignore
+                    else -1
+                    for i in range(shape.shape[1])  # type: ignore
+                )
+                or (1,)
+            )
+        return shape
+
+    def _populate_sample_shapes(
         self,
+        sample_shapes: np.ndarray,
         index: Index,
         sample_shape_provider: Optional[Callable] = None,
-        pad_tensor: bool = False,
-    ) -> Tuple[Optional[int], ...]:
+        flatten: bool = False,
+    ):
         index_0, sample_index = index.values[0], index.values[1:]
-        if (
-            not index_0.subscriptable()
-            and pad_tensor
-            and index_0.value >= self.tensor_length  # type: ignore
-        ):
-            return self.get_empty_sample().shape
-
-        shape = self.shape_interval(index).astuple()
-        if index_0.is_trivial():
-            return shape
-
-        shape = shape[1:]
         sample_indices = list(
             index_0.indices(self._sequence_length or self.num_samples)
         )
         num_samples = len(sample_indices)
 
-        if num_samples == 0:
-            return (0, *shape)
-
         sample_ndim = self.ndim() - 1
-        sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
 
-        if len(sample_index) > sample_ndim:
-            raise IndexError(
-                f"Too many indices for tensor. Tensor is rank {sample_ndim + 1} but {len(sample_index) + 1} indices were provided."
+        for i, idx in enumerate(sample_indices):
+            if self.tensor_meta.htype in ("text", "json"):
+                shape = (1,)
+            elif sample_shape_provider:
+                shape = self._get_sample_shape_from_provider(
+                    sample_shape_provider, idx, sample_index, flatten
+                )
+            else:
+                self.check_link_ready()
+                shape = self.read_shape_for_sample(idx)  # type: ignore
+                # if link verification was not done
+                if len(shape) > sample_ndim:
+                    sample_ndim = len(shape)
+                    sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
+
+            if flatten:
+                start, end = self.sequence_encoder[i]
+                sample_shapes[start:end] = shape
+            else:
+                sample_shapes[i] = shape
+        return sample_shapes
+
+    def _get_total_samples_and_sample_ndim(self, index_0):
+        """Returns total number of samples (including sequence items) and sample ndim using first index"""
+        tensor_ndim = self.ndim()
+        if self.is_sequence:
+            sample_indices = list(index_0.indices(self._sequence_length))
+            num_samples = sum(
+                map(
+                    lambda x: x[1] - x[0],
+                    [self.sequence_encoder[i] for i in sample_indices],
+                )
             )
+            sample_ndim = tensor_ndim - 2
+        else:
+            num_samples = index_0.length(self.num_samples)
+            sample_ndim = tensor_ndim - 1
+        return num_samples, sample_ndim
+
+    def _group_flat_shapes(self, sample_shapes, index_0, sample_ndim):
+        """Groups shapes of flattened sequence items"""
+        sample_indices = list(index_0.indices(self._sequence_length))
+        num_samples = len(sample_indices)
+        try:
+            sample_shapes = sample_shapes[np.newaxis, :].reshape(
+                num_samples, -1, sample_ndim
+            )
+            return sample_shapes
+        except ValueError:
+            sample_shapes_list = []
+            for i in sample_indices:
+                start, end = self.sequence_encoder[i]
+                sample_shapes_list.append(sample_shapes[start:end])
+            return sample_shapes_list
 
-        if None in shape or self.tensor_meta.is_link:
-            for i, idx in enumerate(sample_indices):
-                if self.tensor_meta.htype in ("text", "json"):
-                    shape = (1,)
-                else:
-                    if sample_shape_provider:
-                        try:
-                            shape = sample_shape_provider(idx)  # type: ignore
-                            if isinstance(shape, tuple) and shape == ():
-                                shape = (0,)
-                            if self.is_sequence:
-                                if sample_index and not sample_index[0].subscriptable():
-                                    shape = (1, *tuple(shape[sample_index[0].value].tolist()))  # type: ignore
-                                else:
-                                    is_same = np.all(shape == shape[0, :], axis=0)  # type: ignore
-                                    shape = (len(shape),) + (
-                                        tuple(
-                                            int(shape[0, i])  # type: ignore
-                                            if is_same[i]  # type: ignore
-                                            else -1
-                                            for i in range(shape.shape[1])  # type: ignore
-                                        )
-                                        or (1,)
-                                    )
-
-                        except (
-                            IndexError
-                        ):  # Happens during transforms, sample shape tensor is not populated yet
-                            shape = self.read_shape_for_sample(idx)  # type: ignore
-                    else:
-                        self.check_link_ready()
-                        shape = self.read_shape_for_sample(idx)  # type: ignore
-                        # if link verification was not done
-                        if len(shape) > sample_ndim:
-                            sample_ndim = len(shape)
-                            sample_shapes = np.zeros(
-                                (num_samples, sample_ndim), dtype=np.int32
-                            )
-                    sample_shapes[i] = shape
+    def shapes(
+        self,
+        index: Index,
+        sample_shape_provider: Optional[Callable] = None,
+        pad_tensor: bool = False,
+    ):
+        if len(index) > 1:
+            raise IndexError(f"`.shapes` only accepts indexing on the primary axis.")
+
+        index_0 = index.values[0]
+        num_samples, sample_ndim = self._get_total_samples_and_sample_ndim(index_0)
+
+        sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
+
+        shape = self.shape_interval(index).astuple()[1:]
+
+        if (
+            not index_0.subscriptable()
+            and pad_tensor
+            and index_0.value >= self.tensor_length  # type: ignore
+        ):
+            shape = self.get_empty_sample().shape
+
+        if num_samples > 0 and None in shape or self.tensor_meta.is_link:
+            sample_shapes = self._populate_sample_shapes(
+                sample_shapes,
+                index,
+                sample_shape_provider,
+                flatten=True if self.is_sequence else False,
+            )
+            if self.is_sequence:
+                sample_shapes = self._group_flat_shapes(
+                    sample_shapes, index_0, sample_ndim
+                )
         else:
             sample_shapes[:] = shape
 
+        return sample_shapes
+
+    def _apply_deeper_indexing(self, sample_shapes, num_samples, sample_index):
+        """Applies rest of the indexing to the sample shapes. Inplace operation."""
         squeeze_dims = set()
         for i in range(num_samples):
             for j in range(len(sample_index)):
                 if sample_index[j].subscriptable():
                     if sample_shapes[i, j] != -1:
                         sample_shapes[i, j] = sample_index[j].length(
                             sample_shapes[i, j]
                         )
                 else:
                     squeeze_dims.add(j)
+        return squeeze_dims
 
+    def _sample_shapes_to_shape(self, sample_shapes, squeeze_dims, sample_ndim):
         is_same = np.all(sample_shapes == sample_shapes[0, :], axis=0)
         shape = [  # type: ignore
             int(sample_shapes[0, i])
             if sample_shapes[0, i] != -1 and is_same[i]
             else None
             for i in range(sample_ndim)
         ]
 
+        return tuple(shape[i] for i in range(len(shape)) if i not in squeeze_dims)
+
+    def shape(
+        self,
+        index: Index,
+        sample_shape_provider: Optional[Callable] = None,
+        pad_tensor: bool = False,
+    ) -> Tuple[Optional[int], ...]:
+        tensor_ndim = self.ndim()
+
+        if len(index) > tensor_ndim:
+            raise IndexError(
+                f"Too many indices for tensor. Tensor is rank {tensor_ndim} but {len(index)} indices were provided."
+            )
+
+        index_0, sample_index = index.values[0], index.values[1:]
+        if (
+            not index_0.subscriptable()
+            and pad_tensor
+            and index_0.value >= self.tensor_length  # type: ignore
+        ):
+            return self.get_empty_sample().shape
+
+        shape = self.shape_interval(index).astuple()
+        if index_0.is_trivial():
+            return shape
+
+        num_samples = index_0.length(self._sequence_length or self.num_samples)
+        if num_samples == 0:
+            return shape
+
+        shape = shape[1:]
+        sample_ndim = tensor_ndim - 1
+        sample_shapes = np.zeros((num_samples, sample_ndim), dtype=np.int32)
+
+        if None in shape or self.tensor_meta.is_link:
+            sample_shapes = self._populate_sample_shapes(
+                sample_shapes, index, sample_shape_provider, flatten=False
+            )
+            sample_ndim = sample_shapes.shape[1]
+        else:
+            sample_shapes[:] = shape
+
+        squeeze_dims = self._apply_deeper_indexing(
+            sample_shapes, num_samples, sample_index
+        )
+        shape = self._sample_shapes_to_shape(sample_shapes, squeeze_dims, sample_ndim)
+
         if index_0.subscriptable():
-            shape = [num_samples, *shape]  # type: ignore
+            shape = (num_samples, *shape)  # type: ignore
 
-        return tuple(shape[i] for i in range(len(shape)) if i not in squeeze_dims)
+        return shape
 
     def ndim(self, index: Optional[Index] = None) -> int:
         ndim = len(self.tensor_meta.min_shape) + 1
         if self.is_sequence:
             ndim += 1
         if index:
             for idx in index.values:
```

### Comparing `deeplake-3.5.3/deeplake/core/compression.py` & `deeplake-3.5.4/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/compute/process.py` & `deeplake-3.5.4/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/compute/provider.py` & `deeplake-3.5.4/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/compute/ray.py` & `deeplake-3.5.4/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/compute/serial.py` & `deeplake-3.5.4/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/compute/thread.py` & `deeplake-3.5.4/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/dataset/__init__.py` & `deeplake-3.5.4/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/dataset/dataset.py` & `deeplake-3.5.4/deeplake/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.5.4/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.5.4/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,19 @@
             "checkout", "checkout method cannot be called on a Dataset view."
         )
 
     def _get_tensor_from_root(self, fullpath):
         tensors = self.indra_ds.tensors
         for tensor in tensors:
             if tensor.name == fullpath:
-                deeplake_tensor = self.deeplake_ds.__getattr__(fullpath)
+                deeplake_tensor = None
+                try:
+                    deeplake_tensor = self.deeplake_ds.__getattr__(fullpath)
+                except:
+                    pass
                 indra_tensor = tensor
                 return DeepLakeQueryTensor(deeplake_tensor, indra_tensor)
 
     def pytorch(
         self,
         batch_size: Optional[int] = 1,
         shuffle: bool = False,
@@ -163,24 +167,21 @@
         if hasattr(self, "_view_entry"):
             ret._view_entry = self._view_entry
         return ret
 
     def __getattr__(self, key):
         try:
             return self.__getitem__(key)
-        except:
+        except TensorDoesNotExistError as ke:
             try:
                 return getattr(self.deeplake_ds, key)
-            except:
-                try:
-                    return getattr(self.indra_ds, key)
-                except:
-                    raise AttributeError(
-                        f"'{self.__class__}' object has no attribute '{key}'"
-                    )
+            except AttributeError:
+                raise AttributeError(
+                    f"'{self.__class__}' object has no attribute '{key}'"
+                ) from ke
 
     def __len__(self):
         return len(self.indra_ds)
 
     @deeplake_reporter.record_call
     def dataloader(self):
         """Returns a :class:`~deeplake.enterprise.DeepLakeDataLoader` object. To use this, install deeplake with ``pip install deeplake[enterprise]``.
@@ -259,18 +260,29 @@
     def index(self):
         return self.deeplake_ds.index
 
     def _tensors(
         self, include_hidden: bool = True, include_disabled=True
     ) -> Dict[str, Tensor]:
         """All tensors belonging to this group, including those within sub groups. Always returns the sliced tensors."""
-        version_state = self.version_state
-        group_index = self.group_index
-        all_tensors = self._all_tensors_filtered(include_hidden, include_disabled)
-        return {t: self[posixpath.join(group_index, t)] for t in all_tensors}
+        original_tensors = self.deeplake_ds._tensors(include_hidden, include_disabled)
+        indra_tensors = self.indra_ds.tensors
+        indra_keys = set(t.name for t in indra_tensors)
+        original_tensors = {
+            k: v for k, v in original_tensors.items() if k in indra_keys or v.hidden
+        }
+        original_keys = set(original_tensors.keys())
+        for t in indra_tensors:
+            if t.name in original_keys:
+                original_tensors[t.name] = DeepLakeQueryTensor(
+                    original_tensors[t.name], t
+                )
+            else:
+                original_tensors[t.name] = DeepLakeQueryTensor(None, t)
+        return original_tensors
 
     def __str__(self):
         path_str = ""
         if self.path:
             path_str = f"path='{self.path}', "
 
         mode_str = ""
```

### Comparing `deeplake-3.5.3/deeplake/core/dataset/invalid_view.py` & `deeplake-3.5.4/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/dataset/view_entry.py` & `deeplake-3.5.4/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/fast_forwarding.py` & `deeplake-3.5.4/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/index/index.py` & `deeplake-3.5.4/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/io.py` & `deeplake-3.5.4/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/ipc.py` & `deeplake-3.5.4/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/link_creds.py` & `deeplake-3.5.4/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/linked_chunk_engine.py` & `deeplake-3.5.4/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/linked_sample.py` & `deeplake-3.5.4/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/linked_tiled_sample.py` & `deeplake-3.5.4/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/lock.py` & `deeplake-3.5.4/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/dataset_meta.py` & `deeplake-3.5.4/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.5.4/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.5.4/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.5.4/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/creds.py` & `deeplake-3.5.4/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/pad.py` & `deeplake-3.5.4/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/sequence.py` & `deeplake-3.5.4/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/shape.py` & `deeplake-3.5.4/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/encode/tile.py` & `deeplake-3.5.4/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/meta/tensor_meta.py` & `deeplake-3.5.4/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/partial_reader.py` & `deeplake-3.5.4/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/partial_sample.py` & `deeplake-3.5.4/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/polygon.py` & `deeplake-3.5.4/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/query/autocomplete.py` & `deeplake-3.5.4/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/query/filter.py` & `deeplake-3.5.4/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/query/query.py` & `deeplake-3.5.4/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/sample.py` & `deeplake-3.5.4/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/serialize.py` & `deeplake-3.5.4/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.5.4/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/gcs.py` & `deeplake-3.5.4/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/google_drive.py` & `deeplake-3.5.4/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/local.py` & `deeplake-3.5.4/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/lru_cache.py` & `deeplake-3.5.4/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/memory.py` & `deeplake-3.5.4/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/provider.py` & `deeplake-3.5.4/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/storage/s3.py` & `deeplake-3.5.4/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tensor.py` & `deeplake-3.5.4/deeplake/core/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,20 +476,38 @@
         shape = self.chunk_engine.shape(
             self.index,
             sample_shape_provider=sample_shape_provider,
             pad_tensor=self.pad_tensor,
         )
 
         if len(self.index.values) == 1 and not self.index.values[0].subscriptable():
-            if np.sum(shape) == 0 and self.meta.max_shape:  # type: ignore
+            if None not in shape and np.sum(shape) == 0 and self.meta.max_shape:  # type: ignore
                 shape = (0,) * len(self.meta.max_shape)
         if self.meta.max_shape == [0, 0, 0]:
             shape = ()
         return shape
 
+    def shapes(self):
+        """Get the shapes of all the samples in the tensor.
+
+        Returns:
+            np.ndarray: List of shapes of all the samples in the tensor.
+        """
+        sample_shape_tensor = self._sample_shape_tensor
+        sample_shape_provider = (
+            self._sample_shape_provider(sample_shape_tensor)
+            if sample_shape_tensor
+            else None
+        )
+        return self.chunk_engine.shapes(
+            self.index,
+            sample_shape_provider=sample_shape_provider,
+            pad_tensor=self.pad_tensor,
+        )
+
     @property
     def size(self) -> Optional[int]:
         s = 1
         for x in self.shape:
             if x is None:
                 return None
             s *= x  # not using np.prod to avoid overflow
@@ -940,20 +958,24 @@
             full_arr = self.chunk_engine.numpy(
                 self.index,
                 aslist=False,
                 pad_tensor=self.pad_tensor,
             )
             value = parse_mesh_to_dict(full_arr, self.sample_info)
             return value
-        else:
+        elif hasattr(self, "chunk_engine"):
             return {
                 "value": self.chunk_engine.numpy(
                     index=self.index, aslist=aslist, fetch_chunks=fetch_chunks
                 ),
             }
+        else:
+            return {
+                "value": self.numpy(aslist=aslist, fetch_chunks=fetch_chunks),
+            }
 
     def tobytes(self) -> bytes:
         """Returns the bytes of the tensor.
 
         - Only works for a single sample of tensor.
         - If the tensor is uncompressed, this returns the bytes of the numpy array.
         - If the tensor is sample compressed, this returns the compressed bytes of the sample.
```

### Comparing `deeplake-3.5.3/deeplake/core/tensor_link.py` & `deeplake-3.5.4/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/test_serialize.py` & `deeplake-3.5.4/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_compression.py` & `deeplake-3.5.4/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_compute.py` & `deeplake-3.5.4/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.5.4/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from deeplake.util.exceptions import DynamicTensorNumpyError
 from deeplake.core.dataset.deeplake_query_dataset import DeepLakeQueryDataset
 import random
 import pytest
 
 
 @requires_libdeeplake
-def test_indexing(hub_cloud_ds_generator):
+def test_indexing(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         for i in range(1000):
             deeplake_ds.label.append(int(100 * random.uniform(0.0, 1.0)))
 
     indra_ds = dataset_to_libdeeplake(deeplake_ds)
     deeplake_indra_ds = DeepLakeQueryDataset(deeplake_ds=deeplake_ds, indra_ds=indra_ds)
@@ -49,18 +49,18 @@
 
     assert np.all(
         deeplake_indra_ds[(0, 1),].label.numpy() == indra_ds.label[(0, 1),].numpy()
     )
 
 
 @requires_libdeeplake
-def test_save_view(hub_cloud_ds_generator):
+def test_save_view(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         for i in range(1000):
             deeplake_ds.label.append(int(100 * random.uniform(0.0, 1.0)))
 
     deeplake_ds.commit("First")
 
@@ -70,18 +70,18 @@
     assert (
         deeplake_indra_ds.base_storage["queries.json"]
         == deeplake_ds.base_storage["queries.json"]
     )
 
 
 @requires_libdeeplake
-def test_load_view(hub_cloud_ds_generator):
+def test_load_view(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         deeplake_ds.create_tensor(
             "image", htype="image", dtype=np.uint8, sample_compression="jpg"
         )
         for i in range(100):
             deeplake_ds.label.append(i % 10)
@@ -122,32 +122,33 @@
         iss.append(i)
 
     assert iss == [0, 1, 2]
     assert np.all(indra_ds.image.numpy() == deeplake_indra_ds.image.numpy())
 
 
 @requires_libdeeplake
-def test_query(hub_cloud_ds_generator):
+def test_query(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         deeplake_ds.create_tensor(
             "image", htype="image", dtype=np.uint8, sample_compression="jpg"
         )
         for i in range(100):
             deeplake_ds.label.append(int(i / 10))
             deeplake_ds.image.append(np.random.randint(0, 255, (100, 200, 3), np.uint8))
 
     indra_ds = dataset_to_libdeeplake(deeplake_ds)
     deeplake_indra_ds = DeepLakeQueryDataset(deeplake_ds=deeplake_ds, indra_ds=indra_ds)
 
     view = deeplake_indra_ds.query("SELECT * GROUP BY label")
     assert len(view) == 10
+    assert view.label.shape == view.tensors["label"].shape
     for i in range(len(view)):
         arr = view.label[i].numpy()
         assert len(arr) == 10
         for a in arr:
             assert np.all(a == i)
 
     view2 = view.query("SELECT * WHERE all(label == 2)")
@@ -155,18 +156,18 @@
     arr = view2.label.numpy()
     assert len(arr) == 10
     for a in arr:
         assert np.all(a == 2)
 
 
 @requires_libdeeplake
-def test_metadata(hub_cloud_ds_generator):
+def test_metadata(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         deeplake_ds.create_tensor(
             "image", htype="image", dtype=np.uint8, sample_compression="jpeg"
         )
         deeplake_ds.create_tensor("none_metadata")
         deeplake_ds.create_tensor(
@@ -186,34 +187,34 @@
     assert deeplake_indra_ds.sequence.sample_compression == None
     assert deeplake_indra_ds.none_metadata.htype == None
     assert deeplake_indra_ds.none_metadata.dtype == None
     assert deeplake_indra_ds.none_metadata.sample_compression == None
 
 
 @requires_libdeeplake
-def test_accessing_data(hub_cloud_ds_generator):
+def test_accessing_data(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
-    deeplake_ds = hub_cloud_ds_generator()
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         for i in range(1000):
             deeplake_ds.label.append(int(100 * random.uniform(0.0, 1.0)))
 
     indra_ds = dataset_to_libdeeplake(deeplake_ds)
     deeplake_indra_ds = DeepLakeQueryDataset(deeplake_ds=deeplake_ds, indra_ds=indra_ds)
 
     assert np.all(
         np.isclose(deeplake_indra_ds.label.numpy(), deeplake_indra_ds["label"].numpy())
     )
 
 
 @requires_libdeeplake
-def test_sequences_accessing_data(hub_cloud_ds_generator):
-    deeplake_ds = hub_cloud_ds_generator()
+def test_sequences_accessing_data(local_ds_generator):
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         for i in range(200):
             deeplake_ds.label.append(int(i / 101))
         deeplake_ds.create_tensor(
             "image", htype="image", sample_compression="jpeg", dtype=np.uint8
         )
@@ -232,16 +233,16 @@
     assert deeplake_indra_ds[1, 98].image.shape == [20, 10, 3]
     assert deeplake_indra_ds[1].image.numpy().shape == (99,)
     assert deeplake_indra_ds[1].image.numpy()[0].shape == (10, 10, 3)
     assert deeplake_indra_ds[1].image.numpy()[98].shape == (20, 10, 3)
 
 
 @requires_libdeeplake
-def test_random_split(hub_cloud_ds_generator):
-    deeplake_ds = hub_cloud_ds_generator()
+def test_random_split(local_ds_generator):
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         for i in range(1000):
             deeplake_ds.label.append(int(i % 100))
 
     deeplake_indra_ds = deeplake_ds.query("SELECT * GROUP BY label")
 
@@ -275,36 +276,57 @@
     assert len(val) == 10
     l = val.dataloader().pytorch().shuffle()
     for b in l:
         pass
 
 
 @requires_libdeeplake
-def test_virtual_tensors(hub_cloud_ds_generator):
-    deeplake_ds = hub_cloud_ds_generator()
+def test_virtual_tensors(local_ds_generator):
+    deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         deeplake_ds.create_tensor("embeddings", htype="generic", dtype=np.float32)
+        deeplake_ds.create_tensor("text", htype="text")
+        deeplake_ds.create_tensor("json", htype="json")
         for i in range(100):
             count = i % 5
             deeplake_ds.label.append([int(i % 100)] * count)
             deeplake_ds.embeddings.append(
                 [1.0 / float(i + 1), 0.0, -1.0 / float(i + 1)]
             )
+            deeplake_ds.text.append(f"Hello {i}")
+            deeplake_ds.json.append('{"key": "val"}')
 
     deeplake_indra_ds = deeplake_ds.query("SELECT shape(label)[0] as num_labels")
+    assert np.all(
+        deeplake_indra_ds.num_labels.data()["value"]
+        == deeplake_indra_ds.num_labels.numpy()
+    )
+    assert list(deeplake_indra_ds.tensors.keys()) == ["num_labels"]
     assert len(deeplake_indra_ds) == 100
     assert deeplake_indra_ds.num_labels[0].numpy() == [0]
     assert deeplake_indra_ds.num_labels[1].numpy() == [1]
     assert deeplake_indra_ds.num_labels[2].numpy() == [2]
     assert deeplake_indra_ds.num_labels[3].numpy() == [3]
     assert deeplake_indra_ds.num_labels[4].numpy() == [4]
     assert np.sum(deeplake_indra_ds.num_labels.numpy()) == 200
+    deeplake_indra_ds = deeplake_ds.query("SELECT *, shape(label)[0] as num_labels")
+    assert list(deeplake_indra_ds.tensors.keys()) == [
+        "label",
+        "embeddings",
+        "text",
+        "json",
+        "num_labels",
+    ]
+    assert deeplake_indra_ds.text[0].data() == {"value": "Hello 0"}
+    assert deeplake_indra_ds.json[0].data() == {"value": '{"key": "val"}'}
+    assert deeplake_ds.json[0].data() == {"value": '{"key": "val"}'}
 
     deeplake_indra_ds = deeplake_ds.query(
         "SELECT l2_norm(embeddings - ARRAY[0, 0, 0]) as score order by l2_norm(embeddings - ARRAY[0, 0, 0]) asc"
     )
+    assert list(deeplake_indra_ds.tensors.keys()) == ["score"]
     assert len(deeplake_indra_ds) == 100
     for i in range(100, 1):
         assert deeplake_indra_ds.score[100 - i].numpy() == [
             np.sqrt(2.0 / (i + 1) / (i + 1))
         ]
```

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_io.py` & `deeplake-3.5.4/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_locking.py` & `deeplake-3.5.4/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_readonly.py` & `deeplake-3.5.4/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tests/test_serialize.py` & `deeplake-3.5.4/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/deserialize.py` & `deeplake-3.5.4/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/optimizer.py` & `deeplake-3.5.4/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.5.4/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/serialize.py` & `deeplake-3.5.4/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.5.4/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/tiling/test_serialize.py` & `deeplake-3.5.4/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/transform/test_transform.py` & `deeplake-3.5.4/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/transform/transform.py` & `deeplake-3.5.4/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/transform/transform_dataset.py` & `deeplake-3.5.4/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/transform/transform_tensor.py` & `deeplake-3.5.4/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.5.4/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.5.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 
 
 def embedding_fn(text, embedding_dim=100):
     return np.zeros((len(text), embedding_dim))
 
 
+@pytest.mark.skip(reason="need to update backend")
 @requires_libdeeplake
 @pytest.mark.parametrize("distance_metric", ["L1", "L2", "COS", "MAX", "DOT"])
 def test_search(distance_metric, hub_cloud_dev_token):
     k = 4
     query_embedding = np.random.randint(0, 255, (1, embedding_dim))
 
     # initialize vector store object:
```

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 from typing import Union, List, Any, Optional, Tuple
 
 from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
 from deeplake.core.vectorstore.vector_search.indra import query
-from deeplake.core.vectorstore.vector_search import utils
 from deeplake.core.dataset import Dataset as DeepLakeDataset
 
 
 def vector_search(
     query_embedding: np.ndarray,
     distance_metric: str,
     deeplake_dataset: DeepLakeDataset,
@@ -25,15 +24,14 @@
         k (int): number of samples to return after the search.
         embedding_tensor (str): name of the tensor in the dataset with `htype = "embedding"`.
         **kwargs (Any): Any additional parameters.
 
     Returns:
         Tuple[List, List]: tuple representing the indices of the returned embeddings and their respective scores.
     """
-    from indra import api  # type: ignore
 
     tql_query = query.parse_query(distance_metric, k, query_embedding, embedding_tensor)
     indra_ds = dataset_to_libdeeplake(deeplake_dataset)
 
     view = indra_ds.query(tql_query)
     indices = view.indexes
```

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.5.4/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/commit_diff.py` & `deeplake-3.5.4/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/commit_node.py` & `deeplake-3.5.4/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.5.4/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/test_merge.py` & `deeplake-3.5.4/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/core/version_control/test_version_control.py` & `deeplake-3.5.4/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.5.4/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/enterprise/dataloader.py` & `deeplake-3.5.4/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.5.4/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.5.4/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/enterprise/test_pytorch.py` & `deeplake-3.5.4/deeplake/enterprise/test_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     return sample["index"], sample["xyz"]
 
 
 @requires_torch
 @requires_libdeeplake
 @pytest.mark.parametrize(
     "ds",
-    ["hub_cloud_ds", "hub_cloud_gcs_ds"],
+    ["hub_cloud_ds", "local_ds"],
     indirect=True,
 )
 def test_pytorch_small(ds):
     with ds:
         ds.create_tensor("image", max_chunk_size=PYTORCH_TESTS_MAX_CHUNK_SIZE)
         ds.image.extend(([i * np.ones((i + 1, i + 1)) for i in range(16)]))
         ds.commit()
```

### Comparing `deeplake-3.5.3/deeplake/enterprise/test_query.py` & `deeplake-3.5.4/deeplake/enterprise/test_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,47 +13,45 @@
     dsv = hub_cloud_ds.query("SELECT * WHERE CONTAINS(label, 2)")
     assert len(dsv) == 20
     for i in range(20):
         assert dsv.label[i].numpy() == 2
 
 
 @requires_libdeeplake
-def test_sample(hub_cloud_ds):
-    with hub_cloud_ds as ds:
+def test_sample(local_ds):
+    with local_ds as ds:
         ds.create_tensor("label")
         for i in range(100):
             ds.label.append(floor(i / 20))
 
-    dsv = hub_cloud_ds.sample_by(
+    dsv = local_ds.sample_by(
         "max_weight(label == 2: 10, label == 1: 1)", replace=False, size=10
     )
     assert len(dsv) == 10
     for i in range(10):
         assert dsv.label[i].numpy() == 2 or dsv.label[i].numpy() == 1
 
-    dsv = hub_cloud_ds.sample_by(
-        "max_weight(label == 2: 10, label == 1: 1)", replace=True
-    )
+    dsv = local_ds.sample_by("max_weight(label == 2: 10, label == 1: 1)", replace=True)
     assert len(dsv) == 100
     for i in range(100):
         assert dsv.label[i].numpy() == 2 or dsv.label[i].numpy() == 1
 
-    dsv = hub_cloud_ds.sample_by("label")
+    dsv = local_ds.sample_by("label")
     assert len(dsv) == 100
 
     weights = list()
     for i in range(100):
         weights.append(1 if floor(i / 20) == 0 else 0)
 
-    dsv = hub_cloud_ds.sample_by(weights)
+    dsv = local_ds.sample_by(weights)
     assert len(dsv) == 100
     for i in range(100):
         assert dsv.label[i].numpy() == 0
 
     weights = np.ndarray((100), np.int32)
     for i in range(100):
         weights[i] = 1 if floor(i / 10) == 0 else 0
 
-    dsv = hub_cloud_ds.sample_by(weights)
+    dsv = local_ds.sample_by(weights)
     assert len(dsv) == 100
     for i in range(100):
         assert dsv.label[i].numpy() == 0
```

### Comparing `deeplake-3.5.3/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.5.4/deeplake/enterprise/test_tensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -459,31 +459,27 @@
 def test_tensorflow_ddp():
     raise NotImplementedError
 
 
 @requires_tensorflow
 @requires_libdeeplake
 @pytest.mark.parametrize("compression", [None, "jpeg"])
-def test_tensorflow_decode(hub_cloud_ds, compressed_image_paths, compression):
-    with hub_cloud_ds:
-        hub_cloud_ds.create_tensor("image", sample_compression=compression)
-        hub_cloud_ds.image.extend(
+def test_tensorflow_decode(local_ds, compressed_image_paths, compression):
+    with local_ds:
+        local_ds.create_tensor("image", sample_compression=compression)
+        local_ds.image.extend(
             np.array([i * np.ones((10, 10, 3), dtype=np.uint8) for i in range(5)])
         )
-        hub_cloud_ds.image.extend(
-            [deeplake.read(compressed_image_paths["jpeg"][0])] * 5
-        )
-    if isinstance(
-        get_base_storage(hub_cloud_ds.storage), (MemoryProvider, GCSProvider)
-    ):
+        local_ds.image.extend([deeplake.read(compressed_image_paths["jpeg"][0])] * 5)
+    if isinstance(get_base_storage(local_ds.storage), (MemoryProvider, GCSProvider)):
         with pytest.raises(ValueError):
-            dl = hub_cloud_ds.dataloader()
+            dl = local_ds.dataloader()
         return
 
-    ptds = hub_cloud_ds.dataloader().tensorflow(
+    ptds = local_ds.dataloader().tensorflow(
         collate_fn=identity_collate, decode_method={"image": "tobytes"}
     )
 
     for i, batch in enumerate(ptds):
         image = batch[0]["image"]
         assert isinstance(image, bytes)
         if i < 5 and not compression:
@@ -492,15 +488,15 @@
                 i * np.ones((10, 10, 3), dtype=np.uint8),
             )
         elif i >= 5 and compression:
             with open(compressed_image_paths["jpeg"][0], "rb") as f:
                 assert f.read() == image
 
     if compression:
-        ptds = hub_cloud_ds.dataloader().numpy(decode_method={"image": "pil"})
+        ptds = local_ds.dataloader().numpy(decode_method={"image": "pil"})
         for i, batch in enumerate(ptds):
             image = batch[0]["image"]
             assert isinstance(image, Image.Image)
             if i < 5:
                 np.testing.assert_array_equal(
                     np.array(image), i * np.ones((10, 10, 3), dtype=np.uint8)
                 )
@@ -646,31 +642,31 @@
 
     for batch in ptds:
         assert batch.keys() == {"xyz", "index"}
 
 
 @requires_libdeeplake
 @requires_tensorflow
-def test_uneven_iteration(hub_cloud_ds):
-    with hub_cloud_ds as ds:
+def test_uneven_iteration(local_ds):
+    with local_ds as ds:
         ds.create_tensor("x")
         ds.create_tensor("y")
         ds.x.extend(list(range(5)))
         ds.y.extend(list(range(10)))
     ptds = ds.dataloader().tensorflow()
     for i, batch in enumerate(ptds):
         x, y = np.array(batch["x"][0]), np.array(batch["y"][0])
         np.testing.assert_equal(x, i)
         np.testing.assert_equal(y, i)
 
 
 @requires_libdeeplake
 @requires_tensorflow
-def test_tensorflow_error_handling(hub_cloud_ds):
-    with hub_cloud_ds as ds:
+def test_tensorflow_error_handling(local_ds):
+    with local_ds as ds:
         ds.create_tensor("x")
         ds.create_tensor("y")
         ds.x.extend(list(range(5)))
 
     ptds = ds.dataloader().tensorflow()
     with pytest.raises(EmptyTensorError):
         for _ in ptds:
```

### Comparing `deeplake-3.5.3/deeplake/enterprise/util.py` & `deeplake-3.5.4/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/hooks.py` & `deeplake-3.5.4/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/htype.py` & `deeplake-3.5.4/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.5.4/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/pytorch/common.py` & `deeplake-3.5.4/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.5.4/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.5.4/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.5.4/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/tf/common.py` & `deeplake-3.5.4/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.5.4/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.5.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/integrations/wandb/wandb.py` & `deeplake-3.5.4/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/tests/cache_fixtures.py` & `deeplake-3.5.4/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/tests/client_fixtures.py` & `deeplake-3.5.4/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/tests/common.py` & `deeplake-3.5.4/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/tests/dataset_fixtures.py` & `deeplake-3.5.4/deeplake/tests/dataset_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 
 @pytest.fixture
 def local_ds(local_ds_generator):
     return local_ds_generator()
 
 
 @pytest.fixture
-def local_ds_generator(local_path):
+def local_ds_generator(local_path, hub_cloud_dev_token):
     def generate_local_ds(**kwargs):
-        return deeplake.dataset(local_path, **kwargs)
+        return deeplake.dataset(local_path, token=hub_cloud_dev_token, **kwargs)
 
     return generate_local_ds
 
 
 @pytest.fixture
 def s3_ds(s3_ds_generator):
     return s3_ds_generator()
```

### Comparing `deeplake-3.5.3/deeplake/tests/path_fixtures.py` & `deeplake-3.5.4/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/tests/storage_fixtures.py` & `deeplake-3.5.4/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/access_method.py` & `deeplake-3.5.4/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/agreement.py` & `deeplake-3.5.4/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/array_list.py` & `deeplake-3.5.4/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/assert_byte_indexes.py` & `deeplake-3.5.4/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/auto.py` & `deeplake-3.5.4/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/bugout_reporter.py` & `deeplake-3.5.4/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/cache_chain.py` & `deeplake-3.5.4/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/casting.py` & `deeplake-3.5.4/deeplake/util/casting.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return "generic"
     types = set((map(type, val)))  # type: ignore
     if dict in types:
         return "json"
     if types == set((str,)):
         return "text"
     if object in [  # type: ignore
-        np.array(x).dtype if not isinstance(x, np.ndarray) else x.dtype for x in val  # type: ignore
+        np.array(x).dtype if not isinstance(x, np.ndarray) else x.dtype for x in val if x is not None  # type: ignore
     ]:
         return "json"
     return "generic"
 
 
 def get_empty_text_like_sample(htype: str):
     """Get an empty sample of the given htype.
```

### Comparing `deeplake-3.5.3/deeplake/util/check_latest_version.py` & `deeplake-3.5.4/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/chunk_engine.py` & `deeplake-3.5.4/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/class_label.py` & `deeplake-3.5.4/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/compute.py` & `deeplake-3.5.4/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/connect_dataset.py` & `deeplake-3.5.4/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/dataset.py` & `deeplake-3.5.4/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/diff.py` & `deeplake-3.5.4/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/downsample.py` & `deeplake-3.5.4/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/encoder.py` & `deeplake-3.5.4/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/exceptions.py` & `deeplake-3.5.4/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/exif.py` & `deeplake-3.5.4/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/from_tfds.py` & `deeplake-3.5.4/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/htype.py` & `deeplake-3.5.4/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/image.py` & `deeplake-3.5.4/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/invalid_view_op.py` & `deeplake-3.5.4/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/iteration_warning.py` & `deeplake-3.5.4/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/json.py` & `deeplake-3.5.4/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/keys.py` & `deeplake-3.5.4/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/link.py` & `deeplake-3.5.4/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/logging.py` & `deeplake-3.5.4/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/merge.py` & `deeplake-3.5.4/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/modified.py` & `deeplake-3.5.4/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/notebook.py` & `deeplake-3.5.4/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/mesh.py` & `deeplake-3.5.4/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.5.4/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.5.4/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.5.4/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.5.4/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/path.py` & `deeplake-3.5.4/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/pretty_print.py` & `deeplake-3.5.4/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/remove_cache.py` & `deeplake-3.5.4/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/scheduling.py` & `deeplake-3.5.4/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/shape_interval.py` & `deeplake-3.5.4/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/spinner.py` & `deeplake-3.5.4/deeplake/util/spinner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from deeplake.constants import SPINNER_START_DELAY, SPINNER_ENABLED
 from deeplake.client.log import configure_logger
 from logging import StreamHandler
 from itertools import cycle
 from functools import wraps
 
+import deeplake
 import contextlib
 import threading
 import logging
 import time
 import sys
 
 ACTIVE_SPINNER = None
@@ -28,15 +28,15 @@
         return getattr(self.file, attr)
 
 
 @contextlib.contextmanager
 def run_spinner(spinner):
     global ACTIVE_SPINNER
     try:
-        if not isinstance(sys.stderr, DummyFile) and SPINNER_ENABLED:
+        if not isinstance(sys.stderr, DummyFile) and deeplake.constants.SPINNER_ENABLED:
             spinner.start()
             spinner_started = True
             save_stdout = sys.stdout
             save_stderr = sys.stderr
             sys.stdout = DummyFile(sys.stdout, spinner)
             sys.stderr = DummyFile(sys.stderr, spinner)
             # configure logger to use new stdout
@@ -67,15 +67,15 @@
         self._hide_event = threading.Event()
         self._cur_line_len = 0
         self.daemon = True
         self._stderr_lock = threading.Lock()
         self.file = sys.stderr
 
     def run(self):
-        time.sleep(SPINNER_START_DELAY)
+        time.sleep(deeplake.constants.SPINNER_START_DELAY)
         frames = cycle("/-\\|")
         if not self._hide_event.is_set():
             self._hide_cursor()
         while not self._stop_event.is_set():
             if self._hide_event.is_set():
                 time.sleep(0.1)
                 continue
@@ -128,15 +128,15 @@
             self.file.write("\033[?25h")
             self.file.flush()
 
 
 def spinner(func):
     @wraps(func)
     def inner(*args, **kwargs):
-        if kwargs.get("verbose") in (None, True):
+        if kwargs.pop("spinner", True) and kwargs.get("verbose") in (None, True):
             spinner = Spinner()
 
             with run_spinner(spinner):
                 return func(*args, **kwargs)
         else:
             return func(*args, **kwargs)
```

### Comparing `deeplake-3.5.3/deeplake/util/split.py` & `deeplake-3.5.4/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/storage.py` & `deeplake-3.5.4/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tag.py` & `deeplake-3.5.4/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/testing.py` & `deeplake-3.5.4/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_auto.py` & `deeplake-3.5.4/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.5.4/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.5.4/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_read.py` & `deeplake-3.5.4/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.5.4/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_split.py` & `deeplake-3.5.4/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/tests/test_version_control.py` & `deeplake-3.5.4/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/transform.py` & `deeplake-3.5.4/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/version_control.py` & `deeplake-3.5.4/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/util/video.py` & `deeplake-3.5.4/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/visualizer/video_streaming.py` & `deeplake-3.5.4/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake/visualizer/visualizer.py` & `deeplake-3.5.4/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake.egg-info/PKG-INFO` & `deeplake-3.5.4/deeplake.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.3
+Version: 3.5.4
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
@@ -314,15 +314,15 @@
 
 </details>
 
 
 <details>
   <summary><b>Deep Lake vs Pinecone</b></summary>
   
-Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring serach for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
+Both Deep Lake and Pinecone enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Pinecone is a fully-managed Vector Database that is optimized for highly demanding applications requiring search for billions of vectors. Deep Lake is a serverless. All computations run client-side, which enables users to get started in seconds. Unlike Pinecone, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Pinecone is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
 
 </details>
 
 <details>
   <summary><b>Deep Lake vs Weaviate</b></summary>
   
 Both Deep Lake and Weaviate enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are  architecturally very different. Weaviate is a Vector Database that can be deployed in a managed service or by the user via Kubernetes or Docker. Deep Lake is serverless. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike Weaviate, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. Deep Lake datasets can be visualized and version controlled. Weaviate is limited to light metadata on top of the embeddings and has no visualization. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.3 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.5.4 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
 Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
@@ -159,15 +159,15 @@
 embeddings. ChromaDB is limited to light metadata on top of the embeddings and
 has no visualization. Deep Lake datasets can be visualized and version
 controlled. Deep Lake also has a performant dataloader for fine-tuning your
 Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
 enable users to store and search vectors (embeddings) and offer integrations
 with LangChain and LlamaIndex. However, they are architecturally very
 different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring serach for billions of vectors. Deep
+highly demanding applications requiring search for billions of vectors. Deep
 Lake is a serverless. All computations run client-side, which enables users to
 get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
 raw data such as images, videos, and text, in addition to embeddings. Deep Lake
 datasets can be visualized and version controlled. Pinecone is limited to light
 metadata on top of the embeddings and has no visualization. Deep Lake also has
 a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
 vs Weaviate Both Deep Lake and Weaviate enable users to store and search
```

### Comparing `deeplake-3.5.3/deeplake.egg-info/SOURCES.txt` & `deeplake-3.5.4/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.3/deeplake.egg-info/requires.txt` & `deeplake-3.5.4/deeplake.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 IPython
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
-libdeeplake==0.0.53
+libdeeplake==0.0.54
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -39,15 +39,15 @@
 av>=8.1.0
 
 [dicom]
 nibabel
 pydicom
 
 [enterprise]
-libdeeplake==0.0.53
+libdeeplake==0.0.54
 pyjwt
 
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
```

### Comparing `deeplake-3.5.3/setup.py` & `deeplake-3.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.53"
+    libdeeplake = "libdeeplake==0.0.54"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

