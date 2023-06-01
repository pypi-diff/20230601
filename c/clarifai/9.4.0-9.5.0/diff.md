# Comparing `tmp/clarifai-9.4.0.tar.gz` & `tmp/clarifai-9.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.4.0.tar", last modified: Tue May  2 21:26:34 2023, max compression
+gzip compressed data, was "clarifai-9.5.0.tar", last modified: Thu Jun  1 21:17:43 2023, max compression
```

## Comparing `clarifai-9.4.0.tar` & `clarifai-9.5.0.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.981151 clarifai-9.4.0/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.4.0/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.4.0/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-02 21:26:34.980944 clarifai-9.4.0/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.4.0/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.961242 clarifai-9.4.0/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.962119 clarifai-9.4.0/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.962852 clarifai-9.4.0/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.963352 clarifai-9.4.0/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.964347 clarifai-9.4.0/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965206 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.954199 clarifai-9.4.0/clarifai/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965339 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965571 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.965841 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966006 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966230 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.966497 clarifai-9.4.0/clarifai/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968089 clarifai-9.4.0/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968659 clarifai-9.4.0/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.968990 clarifai-9.4.0/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.4.0/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.4.0/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.961885 clarifai-9.4.0/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     4063 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-05-02 21:26:34.000000 clarifai-9.4.0/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969242 clarifai-9.4.0/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969467 clarifai-9.4.0/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12387 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.969861 clarifai-9.4.0/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.970231 clarifai-9.4.0/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/data_upload/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.970875 clarifai-9.4.0/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1089 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)     9235 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2110 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.971671 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1414 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.955764 clarifai-9.4.0/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.971806 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972043 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972310 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972445 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.972683 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10917 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.978487 clarifai-9.4.0/clarifai_utils/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     5130 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.979930 clarifai-9.4.0/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.4.0/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.4.0/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.980455 clarifai-9.4.0/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.4.0/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4131 2023-03-23 03:08:12.000000 clarifai-9.4.0/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-05-02 21:26:34.980715 clarifai-9.4.0/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.4.0/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3172 2023-01-07 05:29:12.000000 clarifai-9.4.0/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-05-02 21:26:34.981203 clarifai-9.4.0/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)      897 2023-05-02 21:25:56.000000 clarifai-9.4.0/setup.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.016574 clarifai-9.5.0/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-06-01 21:00:24.000000 clarifai-9.5.0/LICENSE
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-01 21:00:24.000000 clarifai-9.5.0/MANIFEST.in
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-01 21:17:43.016454 clarifai-9.5.0/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-06-01 21:00:24.000000 clarifai-9.5.0/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.004344 clarifai-9.5.0/clarifai/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.005120 clarifai-9.5.0/clarifai/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.005724 clarifai-9.5.0/clarifai/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.006110 clarifai-9.5.0/clarifai/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.006851 clarifai-9.5.0/clarifai/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.007593 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.002017 clarifai-9.5.0/clarifai/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.007729 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.007918 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.008221 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.008379 clarifai-9.5.0/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.008595 clarifai-9.5.0/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.008839 clarifai-9.5.0/clarifai/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.010216 clarifai-9.5.0/clarifai/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.010602 clarifai-9.5.0/clarifai/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/modules/pages.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.010751 clarifai-9.5.0/clarifai/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai/urls/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.004887 clarifai-9.5.0/clarifai.egg-info/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-06-01 21:17:42.000000 clarifai-9.5.0/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4038 2023-06-01 21:17:42.000000 clarifai-9.5.0/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-06-01 21:17:42.000000 clarifai-9.5.0/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       21 2023-06-01 21:17:42.000000 clarifai-9.5.0/clarifai.egg-info/requires.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-06-01 21:17:42.000000 clarifai-9.5.0/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.010876 clarifai-9.5.0/clarifai_utils/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.011113 clarifai-9.5.0/clarifai_utils/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12239 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.011489 clarifai-9.5.0/clarifai_utils/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.011814 clarifai-9.5.0/clarifai_utils/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.012392 clarifai-9.5.0/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1693 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10349 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2110 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.013162 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3651 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4856 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6196 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1414 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.003079 clarifai-9.5.0/clarifai_utils/data_upload/examples/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.013301 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.013521 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.013785 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.013904 clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.014110 clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13040 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.014239 clarifai-9.5.0/clarifai_utils/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     5130 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.015273 clarifai-9.5.0/clarifai_utils/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.015696 clarifai-9.5.0/clarifai_utils/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/modules/pages.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4131 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/modules/style.css
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.015834 clarifai-9.5.0/clarifai_utils/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3172 2023-06-01 21:00:24.000000 clarifai-9.5.0/clarifai_utils/urls/helper.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-06-01 21:17:43.016610 clarifai-9.5.0/setup.cfg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      897 2023-06-01 21:02:24.000000 clarifai-9.5.0/setup.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:17:43.016240 clarifai-9.5.0/tests/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2265 2023-06-01 21:00:24.000000 clarifai-9.5.0/tests/test_auth.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3865 2023-06-01 21:00:24.000000 clarifai-9.5.0/tests/test_modules.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3716 2023-06-01 21:00:24.000000 clarifai-9.5.0/tests/test_stub.py
```

### Comparing `clarifai-9.4.0/LICENSE` & `clarifai-9.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/PKG-INFO` & `clarifai-9.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.4.0
+Version: 9.5.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.4.0/README.md` & `clarifai-9.5.0/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/auth/helper.py` & `clarifai-9.5.0/clarifai/auth/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,15 @@
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
     if os.environ.get("CLARIFAI_USER_ID", "") == "":
       raise Exception("You need to set the 'CLARIFAI_USER_ID' env var." + error_description)
     else:
       user_id = os.environ["CLARIFAI_USER_ID"]
-    if os.environ.get("CLARIFAI_APP_ID", "") == "":
-      raise Exception("You need to set the 'CLARIFAI_APP_ID' env var." + error_description)
-    else:
-      app_id = os.environ["CLARIFAI_APP_ID"]
+    app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = ""
     pat = ""
     if os.environ.get("CLARIFAI_SESSION_TOKEN", "") != "":
       token = os.environ["CLARIFAI_SESSION_TOKEN"]
     if os.environ.get("CLARIFAI_PAT", "") != "":
       pat = os.environ["CLARIFAI_PAT"]
     if token == "" and pat == "":
```

### Comparing `clarifai-9.4.0/clarifai/client/abc.py` & `clarifai-9.5.0/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/client/stub.py` & `clarifai-9.5.0/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/base.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/image.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,37 @@
 
 class VisualClassificationDataset(ClarifaiDataset):
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
 
   def create_input_protos(self, image_path: str, labels: List[Union[str, int]], input_id: str,
-                          dataset_id: str, metadata: Struct) -> resources_pb2.Input:
+                          dataset_id: str, geo_info: Union[List[float], None],
+                          metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: image path.
       `labels`: image label(s)
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single row input
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
+
     input_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
             image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
             concepts=[
                 resources_pb2.Concept(
                   id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)\
                 for _label in labels
             ],
             metadata=metadata))
 
@@ -46,17 +52,18 @@
       Input proto iterator
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
+      geo_info = item.geo_info
 
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
-                                             metadata)
+                                             geo_info, metadata)
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
 
 
 class VisualDetectionDataset(ClarifaiDataset):
   """
@@ -64,30 +71,36 @@
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
     self._annotation_protos = []
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
+                          geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: file path to image
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single row input
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
     input_image_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
-            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),), metadata=metadata))
+            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
+            metadata=metadata))
 
     return input_image_proto
 
   def create_annotation_proto(self, label: str, annotations: List, input_id: str,
                               dataset_id: str) -> resources_pb2.Annotation:
     """
     Create an input proto for each bounding box, label input pair.
@@ -129,16 +142,18 @@
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"label": labels, "split": self.split})
+      geo_info = item.geo_info
 
-      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, metadata)
+      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
+                                                   metadata)
       self._all_input_protos.append(input_image_proto)
 
       # iter over bboxes and classes
       # one id could have more than one bbox and label
       for i in range(len(bboxes)):
         input_annot_proto = self.create_annotation_proto(labels[i], bboxes[i], input_id,
                                                          self.dataset_id)
@@ -153,30 +168,36 @@
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
     self._mask_protos = []  # mask or polygon protos
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
+                          geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: absolute image file path
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single input item
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
     input_image_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
-            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),), metadata=metadata))
+            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
+            metadata=metadata))
 
     return input_image_proto
 
   def create_mask_proto(self, label: str, polygons: List[List[float]], input_id: str,
                         dataset_id: str) -> resources_pb2.Annotation:
     """
     Create an input mask proto for an input polygon/mask and label.
@@ -216,16 +237,18 @@
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"label": labels, "split": self.split})
+      geo_info = item.geo_info
 
-      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, metadata)
+      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
+                                                   metadata)
       self._all_input_protos.append(input_image_proto)
 
       ## Iterate over each masked image and create a proto for upload to clarifai
       ## The length of masks/polygons-list and labels must be equal
       for i, _polygon in enumerate(_polygons):
         try:
           input_mask_proto = self.create_mask_proto(labels[i], _polygon, input_id, self.dataset_id)
```

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/text.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.0/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/examples.py` & `clarifai-9.5.0/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/data_upload/upload.py` & `clarifai-9.5.0/clarifai/data_upload/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #! Clarifai data upload
 
 import importlib
 import inspect
 import os
 import sys
-import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
-from typing import Iterator, Optional, Tuple, Union
+from typing import Iterator, List, Optional, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2, service_pb2_grpc
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from tqdm import tqdm
 
 from clarifai.client import create_stub
 from clarifai.data_upload.datasets.base import Chunker
@@ -85,15 +84,15 @@
       app_id: str,
       pat: str,
       dataset_id: str,
       task: str,
       from_module: Optional[Union[str, os.PathLike]] = None,
       from_zoo: Optional[str] = None,  # load dataset from zoo
       split: str = "train",  # train or test/val
-      chunk_size: int = 16,
+      chunk_size: int = 128,
       portal: str = "clarifai"):
     """
     Initialize upload configs.
     Args:
       `user_id`: Clarifai user id.
       `app_id`: Clarifai app id.
       `pat`: Clarifai PAT(Personal Access Token).
@@ -111,16 +110,16 @@
     self.APP_ID = app_id
     self.PAT = pat
     self.dataset_id = dataset_id
     self.task = task
     self.module_dir = from_module
     self.zoo_dataset = from_zoo
     self.split = split
-    self.chunk_size = chunk_size
-    self.num_workers: int = cpu_count()
+    self.chunk_size = min(128, chunk_size)  # limit max protos in a req
+    self.num_workers: int = min(10, cpu_count())  #15 req/sec rate limit
     self.__base: str = ""
     if portal == "dev":
       self.__base = "https://api-dev.clarifai.com"
     elif portal == "staging":
       self.__base = "https://api-staging.clarifai.com"
     else:  #prod
       self.__base = "https://api.clarifai.com"
@@ -131,105 +130,144 @@
     os.environ["CLARIFAI_API_BASE"] = self.__base
     os.environ["CLARIFAI_PAT"] = self.PAT
 
     self.STUB: service_pb2_grpc.V2Stub = create_stub()
     self.metadata: Tuple = (('authorization', 'Key ' + self.PAT),)
     self.user_app_id = resources_pb2.UserAppIDSet(user_id=self.USER_ID, app_id=self.APP_ID)
 
-  def _upload_inputs(self, inputs):
+  def _upload_inputs(self, batch_input: List[resources_pb2.Input]
+                    ) -> Union[List[resources_pb2.Input], List[None]]:
     """
     Upload inputs to clarifai platform dataset.
     Args:
-      inputs: input protos
+      batch_input: input batch protos
+    Returns:
+      retry_upload: failed input upload
     """
-    upload_count = 0
     retry_upload = []  # those that fail to upload are stored for retries
+    response = self.STUB.PostInputs(
+        service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=batch_input),)
 
-    for inp_proto in inputs:
-      response = self.STUB.PostInputs(
-          service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=[inp_proto]),)
-
-      MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
-      if response.status.code != status_code_pb2.SUCCESS:
-        try:
-          if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
-            retry_upload.append(inp_proto)
-          print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
-          continue
-        except:
-          print(f"Post inputs failed, status: {response.status.details}\n")
-      else:
-        upload_count += 1
+    MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
+    if response.status.code != status_code_pb2.SUCCESS:
+      try:
+        if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
+          retry_upload.extend(batch_input)
+        print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
+      except:
+        if "Duplicated inputs ID" not in response.status.details:
+          retry_upload.extend(batch_input)
+        print(f"Post inputs failed, status: {response.status.details}\n")
 
     return retry_upload
 
-  def upload_annotations(self, inputs):
+  def upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
+                        ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Upload image annotations to clarifai detection dataset
+    Args:
+      batch_annot: annot batch protos
+    Returns:
+      retry_upload: failed annot upload
     """
-    upload_count = 0
     retry_upload = []  # those that fail to upload are stored for retries
+    response = self.STUB.PostAnnotations(
+        service_pb2.PostAnnotationsRequest(user_app_id=self.user_app_id, annotations=batch_annot),)
 
-    for annot_proto in inputs:
-      response = self.STUB.PostAnnotations(
-          service_pb2.PostAnnotationsRequest(
-              user_app_id=self.user_app_id, annotations=[annot_proto]),)
-
-      if response.status.code != status_code_pb2.SUCCESS:
-        try:
-          print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
-          continue
-        except:
-          print(f"Post annotations failed, status:\n{response.status.details}\n")
-          retry_upload.append(annot_proto)
-      else:
-        upload_count += 1
+    if response.status.code != status_code_pb2.SUCCESS:
+      try:
+        print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
+      except:
+        print(f"Post annotations failed, status:\n{response.status.details}\n")
+      finally:
+        retry_upload.extend(batch_annot)
 
     return retry_upload
 
-  def concurrent_inp_upload(self, inputs, chunks):
+  def concurrent_inp_upload(
+      self,
+      inputs: List[List[resources_pb2.Input]],
+      chunks: int,
+      desc: str = "uploading inputs...") -> Union[List[resources_pb2.Input], List[None]]:
     """
     Upload images concurrently.
+    Args:
+      inputs: input protos
+      chunks: number of inputs chunks
+    Returns:
+      retry_upload: All failed input protos during upload
     """
     inp_threads = []
     retry_upload = []
 
     with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      for inp_batch in tqdm(inputs, total=chunks + 1, desc="uploading inputs..."):
-        inp_threads.append(executor.submit(self._upload_inputs, inp_batch))
-        time.sleep(0.1)
-
-    for job in tqdm(
-        as_completed(inp_threads), total=chunks + 1, desc="retry uploading failed protos..."):
-      if job.result():
-        retry_upload.extend(job.result())
-
-    if len(
-        list(retry_upload)) > 0:  ## TODO: use api_with_retries functionality via upload_inputs()
-      _ = self._upload_inputs(retry_upload)
+      with tqdm(total=chunks, desc=desc) as progress:
+        # Submit all jobs to the executor and store the returned futures
+        inp_threads = [executor.submit(self._upload_inputs, inp_batch) for inp_batch in inputs]
+
+        for job in as_completed(inp_threads):
+          result = job.result()
+          if result:
+            retry_upload.extend(result)
+          progress.update()
 
-  def concurrent_annot_upload(self, inputs, chunks):
+    return retry_upload
+
+  def concurrent_annot_upload(
+      self,
+      annots: List[List[resources_pb2.Annotation]],
+      chunks: int,
+      desc: str = "uploading annotations...") -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Uploads annotations concurrently.
+    Args:
+      annots: annot protos
+      chunks: number of annots chunks
+    Returns:
+      retry_annot_upload: All failed annot protos during upload
     """
     annot_threads = []
     retry_annot_upload = []
 
     with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      for annot_batch in tqdm(inputs, total=chunks + 1, desc="uploading..."):
-        annot_threads.append(executor.submit(self.upload_annotations, annot_batch))
-        time.sleep(0.2)
-
-    for job in tqdm(
-        as_completed(annot_threads), total=chunks + 1, desc="retry uploading failed protos..."):
-      if job.result():
-        retry_annot_upload.extend(job.result())
-    if len(retry_annot_upload) > 0:
-      ## TODO: use api_with_retries functionality via upload_annotations()
-      _ = self.upload_annotations(retry_annot_upload)
+      with tqdm(total=chunks, desc=desc) as progress:
+        # Submit all jobs to the executor and store the returned futures
+        annot_threads = [
+            executor.submit(self.upload_annotations, inp_batch) for inp_batch in annots
+        ]
+
+        for job in as_completed(annot_threads):
+          result = job.result()
+          if result:
+            retry_annot_upload.extend(result)
+          progress.update()
+
+    return retry_annot_upload
+
+  def retry_concurrent_uploads(
+      self,
+      retry_upload_protos: Union[List[resources_pb2.Input], List[resources_pb2.Annotation]],
+      upload_type: str = "input") -> None:
+    """
+    Retry Uploads of inputs/annotations.
+    Args:
+      retry_upload_protos: upload protos for retry
+      upload_type: input/annot protos type
+    """
+    retry_chunked_upload_protos = Chunker(retry_upload_protos, self.chunk_size).chunk()
+    if len(retry_upload_protos) > 0 and upload_type == "input":
+      _ = self.concurrent_inp_upload(
+          retry_chunked_upload_protos,
+          len(retry_chunked_upload_protos),
+          desc="retry uploading failed input protos...")
+    elif len(retry_upload_protos) > 0 and upload_type == "annot":
+      _ = self.concurrent_annot_upload(
+          retry_chunked_upload_protos,
+          len(retry_chunked_upload_protos),
+          desc="retry uploading failed annotation protos...")
 
   def upload_to_clarifai(self):
     """
     Execute data upload.
     """
     datagen_object = None
     if self.module_dir is None and self.zoo_dataset is None:
@@ -245,58 +283,57 @@
 
     if self.task == "text_clf":
       dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
       text_protos = dataset_obj._get_input_protos()
       text_protos = dataset_obj._to_list(text_protos)
 
       # Upload text
-      chunks = len(text_protos) // self.num_workers
       chunked_text_protos = Chunker(text_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_text_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_text_protos,
+                                                       len(chunked_text_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
     elif self.task == "visual_detection":
       dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
       img_protos, annotation_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_img_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
       # Upload annotations:
       print("Uploading annotations.......")
       annotation_protos = dataset_obj._to_list(annotation_protos)
-      chunks_ = len(annotation_protos) // self.num_workers
       chunked_annot_protos = Chunker(annotation_protos, self.chunk_size).chunk()
-
-      self.concurrent_annot_upload(chunked_annot_protos, chunks_)
+      retry_upload_protos = self.concurrent_annot_upload(chunked_annot_protos,
+                                                         len(chunked_annot_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "annot")
 
     elif self.task == "visual_segmentation":
       dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
       img_protos, mask_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
       mask_protos = dataset_obj._to_list(mask_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
-      #self.concurrent_inp_upload(chunked_img_protos, chunks)
       # Upload masks:
       print("Uploading masks.......")
-      chunks_ = len(mask_protos) // self.num_workers
       chunked_mask_protos = Chunker(mask_protos, self.chunk_size).chunk()
+      retry_upload_protos = self.concurrent_annot_upload(chunked_mask_protos,
+                                                         len(chunked_mask_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "annot")
 
-      self.concurrent_annot_upload(chunked_mask_protos, chunks_)
     else:  # visual-classification & visual-captioning
       dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
       img_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_img_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
```

### Comparing `clarifai-9.4.0/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.0/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/concepts.py` & `clarifai-9.5.0/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/datasets.py` & `clarifai-9.5.0/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/inputs.py` & `clarifai-9.5.0/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/installed_module_versions.py` & `clarifai-9.5.0/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/lister.py` & `clarifai-9.5.0/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/models.py` & `clarifai-9.5.0/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/module_versions.py` & `clarifai-9.5.0/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/listing/modules.py` & `clarifai-9.5.0/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/modules/css.py` & `clarifai-9.5.0/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/modules/pages.py` & `clarifai-9.5.0/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/modules/style.css` & `clarifai-9.5.0/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai/urls/helper.py` & `clarifai-9.5.0/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai.egg-info/PKG-INFO` & `clarifai-9.5.0/clarifai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.4.0
+Version: 9.5.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.4.0/clarifai.egg-info/SOURCES.txt` & `clarifai-9.5.0/clarifai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 clarifai/listing/lister.py
 clarifai/listing/models.py
 clarifai/listing/module_versions.py
 clarifai/listing/modules.py
 clarifai/modules/__init__.py
 clarifai/modules/css.py
 clarifai/modules/pages.py
-clarifai/modules/style.css
-clarifai/urls/__init__.py
 clarifai/urls/helper.py
 clarifai_utils/__init__.py
 clarifai_utils/auth/__init__.py
 clarifai_utils/auth/helper.py
 clarifai_utils/client/__init__.py
 clarifai_utils/client/abc.py
 clarifai_utils/client/stub.py
@@ -89,9 +87,11 @@
 clarifai_utils/listing/models.py
 clarifai_utils/listing/module_versions.py
 clarifai_utils/listing/modules.py
 clarifai_utils/modules/__init__.py
 clarifai_utils/modules/css.py
 clarifai_utils/modules/pages.py
 clarifai_utils/modules/style.css
-clarifai_utils/urls/__init__.py
-clarifai_utils/urls/helper.py
+clarifai_utils/urls/helper.py
+tests/test_auth.py
+tests/test_modules.py
+tests/test_stub.py
```

### Comparing `clarifai-9.4.0/clarifai_utils/auth/helper.py` & `clarifai-9.5.0/clarifai_utils/auth/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,15 @@
  - 'CLARIFAI_API_BASE': the base domain for the API such as https://api.clarifai.com
  - 'CLARIFAI_UI': the overall UI domain for redirects such as https://clarifai.com
 """
     if os.environ.get("CLARIFAI_USER_ID", "") == "":
       raise Exception("You need to set the 'CLARIFAI_USER_ID' env var." + error_description)
     else:
       user_id = os.environ["CLARIFAI_USER_ID"]
-    if os.environ.get("CLARIFAI_APP_ID", "") == "":
-      raise Exception("You need to set the 'CLARIFAI_APP_ID' env var." + error_description)
-    else:
-      app_id = os.environ["CLARIFAI_APP_ID"]
+    app_id = os.environ.get("CLARIFAI_APP_ID", "")
     token = ""
     pat = ""
     if os.environ.get("CLARIFAI_SESSION_TOKEN", "") != "":
       token = os.environ["CLARIFAI_SESSION_TOKEN"]
     if os.environ.get("CLARIFAI_PAT", "") != "":
       pat = os.environ["CLARIFAI_PAT"]
     if token == "" and pat == "":
```

### Comparing `clarifai-9.4.0/clarifai_utils/client/abc.py` & `clarifai-9.5.0/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/client/stub.py` & `clarifai-9.5.0/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/base.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/base.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,37 @@
 
 class VisualClassificationDataset(ClarifaiDataset):
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
 
   def create_input_protos(self, image_path: str, labels: List[Union[str, int]], input_id: str,
-                          dataset_id: str, metadata: Struct) -> resources_pb2.Input:
+                          dataset_id: str, geo_info: Union[List[float], None],
+                          metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: image path.
       `labels`: image label(s)
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single row input
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
+
     input_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
             image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
             concepts=[
                 resources_pb2.Concept(
                   id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)\
                 for _label in labels
             ],
             metadata=metadata))
 
@@ -46,17 +52,18 @@
       Input proto iterator
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
+      geo_info = item.geo_info
 
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
-                                             metadata)
+                                             geo_info, metadata)
       self._all_input_protos.append(input_proto)
 
     return iter(self._all_input_protos)
 
 
 class VisualDetectionDataset(ClarifaiDataset):
   """
@@ -64,30 +71,36 @@
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
     self._annotation_protos = []
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
+                          geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: file path to image
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single row input
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
     input_image_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
-            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),), metadata=metadata))
+            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
+            metadata=metadata))
 
     return input_image_proto
 
   def create_annotation_proto(self, label: str, annotations: List, input_id: str,
                               dataset_id: str) -> resources_pb2.Annotation:
     """
     Create an input proto for each bounding box, label input pair.
@@ -129,16 +142,18 @@
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"label": labels, "split": self.split})
+      geo_info = item.geo_info
 
-      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, metadata)
+      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
+                                                   metadata)
       self._all_input_protos.append(input_image_proto)
 
       # iter over bboxes and classes
       # one id could have more than one bbox and label
       for i in range(len(bboxes)):
         input_annot_proto = self.create_annotation_proto(labels[i], bboxes[i], input_id,
                                                          self.dataset_id)
@@ -153,30 +168,36 @@
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
     self._mask_protos = []  # mask or polygon protos
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
+                          geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
       `image_path`: absolute image file path
       `input_id: unique input id
       `dataset_id`: Clarifai dataset id
+      `geo_info`: image longitude, latitude info
       `metadata`: image metadata
     Returns:
       An input proto representing a single input item
     """
+    geo_pb = resources_pb2.Geo(geo_point=resources_pb2.GeoPoint(
+        longitude=geo_info[0], latitude=geo_info[1])) if geo_info is not None else None
     input_image_proto = resources_pb2.Input(
         id=input_id,
         dataset_ids=[dataset_id],
         data=resources_pb2.Data(
-            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),), metadata=metadata))
+            image=resources_pb2.Image(base64=open(image_path, 'rb').read(),),
+            geo=geo_pb,
+            metadata=metadata))
 
     return input_image_proto
 
   def create_mask_proto(self, label: str, polygons: List[List[float]], input_id: str,
                         dataset_id: str) -> resources_pb2.Annotation:
     """
     Create an input mask proto for an input polygon/mask and label.
@@ -216,16 +237,18 @@
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"label": labels, "split": self.split})
+      geo_info = item.geo_info
 
-      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, metadata)
+      input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
+                                                   metadata)
       self._all_input_protos.append(input_image_proto)
 
       ## Iterate over each masked image and create a proto for upload to clarifai
       ## The length of masks/polygons-list and labels must be equal
       for i, _polygon in enumerate(_polygons):
         try:
           input_mask_proto = self.create_mask_proto(labels[i], _polygon, input_id, self.dataset_id)
```

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/text.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.5.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.5.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.5.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/examples.py` & `clarifai-9.5.0/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/data_upload/upload.py` & `clarifai-9.5.0/clarifai_utils/data_upload/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #! Clarifai data upload
 
 import importlib
 import inspect
 import os
 import sys
-import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
-from typing import Iterator, Optional, Tuple, Union
+from typing import Iterator, List, Optional, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2, service_pb2_grpc
 from clarifai_grpc.grpc.api.status import status_code_pb2
 from tqdm import tqdm
 
 from clarifai.client import create_stub
 from clarifai.data_upload.datasets.base import Chunker
@@ -85,15 +84,15 @@
       app_id: str,
       pat: str,
       dataset_id: str,
       task: str,
       from_module: Optional[Union[str, os.PathLike]] = None,
       from_zoo: Optional[str] = None,  # load dataset from zoo
       split: str = "train",  # train or test/val
-      chunk_size: int = 16,
+      chunk_size: int = 128,
       portal: str = "clarifai"):
     """
     Initialize upload configs.
     Args:
       `user_id`: Clarifai user id.
       `app_id`: Clarifai app id.
       `pat`: Clarifai PAT(Personal Access Token).
@@ -111,16 +110,16 @@
     self.APP_ID = app_id
     self.PAT = pat
     self.dataset_id = dataset_id
     self.task = task
     self.module_dir = from_module
     self.zoo_dataset = from_zoo
     self.split = split
-    self.chunk_size = chunk_size
-    self.num_workers: int = cpu_count()
+    self.chunk_size = min(128, chunk_size)  # limit max protos in a req
+    self.num_workers: int = min(10, cpu_count())  #15 req/sec rate limit
     self.__base: str = ""
     if portal == "dev":
       self.__base = "https://api-dev.clarifai.com"
     elif portal == "staging":
       self.__base = "https://api-staging.clarifai.com"
     else:  #prod
       self.__base = "https://api.clarifai.com"
@@ -131,105 +130,144 @@
     os.environ["CLARIFAI_API_BASE"] = self.__base
     os.environ["CLARIFAI_PAT"] = self.PAT
 
     self.STUB: service_pb2_grpc.V2Stub = create_stub()
     self.metadata: Tuple = (('authorization', 'Key ' + self.PAT),)
     self.user_app_id = resources_pb2.UserAppIDSet(user_id=self.USER_ID, app_id=self.APP_ID)
 
-  def _upload_inputs(self, inputs):
+  def _upload_inputs(self, batch_input: List[resources_pb2.Input]
+                    ) -> Union[List[resources_pb2.Input], List[None]]:
     """
     Upload inputs to clarifai platform dataset.
     Args:
-      inputs: input protos
+      batch_input: input batch protos
+    Returns:
+      retry_upload: failed input upload
     """
-    upload_count = 0
     retry_upload = []  # those that fail to upload are stored for retries
+    response = self.STUB.PostInputs(
+        service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=batch_input),)
 
-    for inp_proto in inputs:
-      response = self.STUB.PostInputs(
-          service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=[inp_proto]),)
-
-      MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
-      if response.status.code != status_code_pb2.SUCCESS:
-        try:
-          if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
-            retry_upload.append(inp_proto)
-          print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
-          continue
-        except:
-          print(f"Post inputs failed, status: {response.status.details}\n")
-      else:
-        upload_count += 1
+    MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
+    if response.status.code != status_code_pb2.SUCCESS:
+      try:
+        if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
+          retry_upload.extend(batch_input)
+        print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
+      except:
+        if "Duplicated inputs ID" not in response.status.details:
+          retry_upload.extend(batch_input)
+        print(f"Post inputs failed, status: {response.status.details}\n")
 
     return retry_upload
 
-  def upload_annotations(self, inputs):
+  def upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
+                        ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Upload image annotations to clarifai detection dataset
+    Args:
+      batch_annot: annot batch protos
+    Returns:
+      retry_upload: failed annot upload
     """
-    upload_count = 0
     retry_upload = []  # those that fail to upload are stored for retries
+    response = self.STUB.PostAnnotations(
+        service_pb2.PostAnnotationsRequest(user_app_id=self.user_app_id, annotations=batch_annot),)
 
-    for annot_proto in inputs:
-      response = self.STUB.PostAnnotations(
-          service_pb2.PostAnnotationsRequest(
-              user_app_id=self.user_app_id, annotations=[annot_proto]),)
-
-      if response.status.code != status_code_pb2.SUCCESS:
-        try:
-          print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
-          continue
-        except:
-          print(f"Post annotations failed, status:\n{response.status.details}\n")
-          retry_upload.append(annot_proto)
-      else:
-        upload_count += 1
+    if response.status.code != status_code_pb2.SUCCESS:
+      try:
+        print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
+      except:
+        print(f"Post annotations failed, status:\n{response.status.details}\n")
+      finally:
+        retry_upload.extend(batch_annot)
 
     return retry_upload
 
-  def concurrent_inp_upload(self, inputs, chunks):
+  def concurrent_inp_upload(
+      self,
+      inputs: List[List[resources_pb2.Input]],
+      chunks: int,
+      desc: str = "uploading inputs...") -> Union[List[resources_pb2.Input], List[None]]:
     """
     Upload images concurrently.
+    Args:
+      inputs: input protos
+      chunks: number of inputs chunks
+    Returns:
+      retry_upload: All failed input protos during upload
     """
     inp_threads = []
     retry_upload = []
 
     with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      for inp_batch in tqdm(inputs, total=chunks + 1, desc="uploading inputs..."):
-        inp_threads.append(executor.submit(self._upload_inputs, inp_batch))
-        time.sleep(0.1)
-
-    for job in tqdm(
-        as_completed(inp_threads), total=chunks + 1, desc="retry uploading failed protos..."):
-      if job.result():
-        retry_upload.extend(job.result())
-
-    if len(
-        list(retry_upload)) > 0:  ## TODO: use api_with_retries functionality via upload_inputs()
-      _ = self._upload_inputs(retry_upload)
+      with tqdm(total=chunks, desc=desc) as progress:
+        # Submit all jobs to the executor and store the returned futures
+        inp_threads = [executor.submit(self._upload_inputs, inp_batch) for inp_batch in inputs]
+
+        for job in as_completed(inp_threads):
+          result = job.result()
+          if result:
+            retry_upload.extend(result)
+          progress.update()
 
-  def concurrent_annot_upload(self, inputs, chunks):
+    return retry_upload
+
+  def concurrent_annot_upload(
+      self,
+      annots: List[List[resources_pb2.Annotation]],
+      chunks: int,
+      desc: str = "uploading annotations...") -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Uploads annotations concurrently.
+    Args:
+      annots: annot protos
+      chunks: number of annots chunks
+    Returns:
+      retry_annot_upload: All failed annot protos during upload
     """
     annot_threads = []
     retry_annot_upload = []
 
     with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      for annot_batch in tqdm(inputs, total=chunks + 1, desc="uploading..."):
-        annot_threads.append(executor.submit(self.upload_annotations, annot_batch))
-        time.sleep(0.2)
-
-    for job in tqdm(
-        as_completed(annot_threads), total=chunks + 1, desc="retry uploading failed protos..."):
-      if job.result():
-        retry_annot_upload.extend(job.result())
-    if len(retry_annot_upload) > 0:
-      ## TODO: use api_with_retries functionality via upload_annotations()
-      _ = self.upload_annotations(retry_annot_upload)
+      with tqdm(total=chunks, desc=desc) as progress:
+        # Submit all jobs to the executor and store the returned futures
+        annot_threads = [
+            executor.submit(self.upload_annotations, inp_batch) for inp_batch in annots
+        ]
+
+        for job in as_completed(annot_threads):
+          result = job.result()
+          if result:
+            retry_annot_upload.extend(result)
+          progress.update()
+
+    return retry_annot_upload
+
+  def retry_concurrent_uploads(
+      self,
+      retry_upload_protos: Union[List[resources_pb2.Input], List[resources_pb2.Annotation]],
+      upload_type: str = "input") -> None:
+    """
+    Retry Uploads of inputs/annotations.
+    Args:
+      retry_upload_protos: upload protos for retry
+      upload_type: input/annot protos type
+    """
+    retry_chunked_upload_protos = Chunker(retry_upload_protos, self.chunk_size).chunk()
+    if len(retry_upload_protos) > 0 and upload_type == "input":
+      _ = self.concurrent_inp_upload(
+          retry_chunked_upload_protos,
+          len(retry_chunked_upload_protos),
+          desc="retry uploading failed input protos...")
+    elif len(retry_upload_protos) > 0 and upload_type == "annot":
+      _ = self.concurrent_annot_upload(
+          retry_chunked_upload_protos,
+          len(retry_chunked_upload_protos),
+          desc="retry uploading failed annotation protos...")
 
   def upload_to_clarifai(self):
     """
     Execute data upload.
     """
     datagen_object = None
     if self.module_dir is None and self.zoo_dataset is None:
@@ -245,58 +283,57 @@
 
     if self.task == "text_clf":
       dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
       text_protos = dataset_obj._get_input_protos()
       text_protos = dataset_obj._to_list(text_protos)
 
       # Upload text
-      chunks = len(text_protos) // self.num_workers
       chunked_text_protos = Chunker(text_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_text_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_text_protos,
+                                                       len(chunked_text_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
     elif self.task == "visual_detection":
       dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
       img_protos, annotation_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_img_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
       # Upload annotations:
       print("Uploading annotations.......")
       annotation_protos = dataset_obj._to_list(annotation_protos)
-      chunks_ = len(annotation_protos) // self.num_workers
       chunked_annot_protos = Chunker(annotation_protos, self.chunk_size).chunk()
-
-      self.concurrent_annot_upload(chunked_annot_protos, chunks_)
+      retry_upload_protos = self.concurrent_annot_upload(chunked_annot_protos,
+                                                         len(chunked_annot_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "annot")
 
     elif self.task == "visual_segmentation":
       dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
       img_protos, mask_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
       mask_protos = dataset_obj._to_list(mask_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
 
-      #self.concurrent_inp_upload(chunked_img_protos, chunks)
       # Upload masks:
       print("Uploading masks.......")
-      chunks_ = len(mask_protos) // self.num_workers
       chunked_mask_protos = Chunker(mask_protos, self.chunk_size).chunk()
+      retry_upload_protos = self.concurrent_annot_upload(chunked_mask_protos,
+                                                         len(chunked_mask_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "annot")
 
-      self.concurrent_annot_upload(chunked_mask_protos, chunks_)
     else:  # visual-classification & visual-captioning
       dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
       img_protos = dataset_obj._get_input_protos()
       img_protos = dataset_obj._to_list(img_protos)
 
       # Upload images
-      chunks = len(img_protos) // self.num_workers
       chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-
-      self.concurrent_inp_upload(chunked_img_protos, chunks)
+      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
+      self.retry_concurrent_uploads(retry_upload_protos, "input")
```

### Comparing `clarifai-9.4.0/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.5.0/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/concepts.py` & `clarifai-9.5.0/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/datasets.py` & `clarifai-9.5.0/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/inputs.py` & `clarifai-9.5.0/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.5.0/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/lister.py` & `clarifai-9.5.0/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/models.py` & `clarifai-9.5.0/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/module_versions.py` & `clarifai-9.5.0/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/listing/modules.py` & `clarifai-9.5.0/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/modules/css.py` & `clarifai-9.5.0/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/modules/pages.py` & `clarifai-9.5.0/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/clarifai_utils/urls/helper.py` & `clarifai-9.5.0/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.4.0/setup.py` & `clarifai-9.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.4.0",
+    version="9.5.0",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
@@ -20,10 +20,10 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license="Apache 2.0",
     python_requires='>=3.8',
     install_requires=[
-        "clarifai-grpc>=9.4.0",
+        "clarifai-grpc>=9.5.0",
     ],
     include_package_data=True)
```

